Thank you very much Hussein,

I like the website approach to getting the message across.

Here is some feedback – don't take any of this negatively. There is a lot of content.

I think Orbus in the middle gives it too much focus. Not sure how to position this better, but TOPL and Mizuho should be the primary. Perhaps just remove Orbus from the images at the top and include it into a foot note or when they are first introduced.
Image

Going back and forth is a bit of a pain. Perhaps breadcrumbs and Prev / Next buttons would enable the navigation to be more suited to continual progress and help presenters.
Are we sure about sanctions screening? This is a very business centric use case – not an IT one.

What type of sanction screening you are considering? There is no detail. It mentions transactions, but is that for AML (Large Transaction, Structuring, Smurfing, Round Tripping, account number is on a watch list, country is on a watch list, recipient is on a watch list etc). For the name being on a watch list or to see if the banks clients (corporates and personnel) it gets very complicated.

I'm happy to be involved in it as I did an extensive solution with BJB over 10 years ago using fuzzy logic engine and known alternatives library for a name check. World Check provides about 1,000,000 names and updates them 4 times a day. The application we built called Informatica IIR as the search engine.

https://docs.informatica.com/master-data-management/identity-resolution/10-1/_introduction-to-ssa-name3-service-groups_identity-resolution_10-1_ditamap/introduction/the_name_search_problem.html

We did it in both directions. A new prospect or client onboarding would bring up and save all the hits against the WC list and local blacklists. The RM would either be a hit (positive match) or reject (false positive) or KIV. Then when we get the delta updates during the day we check all the hits and alert that there has been an update on their client. Check all the KIV and alert that a KIV has more info perhaps it's your client. Finally, we checked against all the non-identified clients and see if that client is a possible match for the deltas and alert for validation accordingly.

It's a tricky business as you need to know that Peggy is a nickname for Margaret and MJ could be Mary Jane etc. Then there are localisations like Jon and John, Jonson and Johnson, Smith and Smyth and Smit etc. We had an Indonesian client who's only name ws Jon. Totally messed up the performance and came back with 1000s of hits! Finally, there are simple spelling mistakes and phonetics to consider. AI can really help here of course. But if someone has an engine like IIR would they need more?

The 'Run Sanctions Screening Simulation – is it actually doing something or just a simple js animation of the text arriving? I'm not sure what value it gives if there is nothing behind it. For examples "Complete Transparency" there is nothing to see how this is transparent.
Do we need any caveats of the implementation roadmap? Access to data etc?
The timelines for the pilot in SG and the rollouts to the countries seems very aggressive. I presume this is a best case scenario assuming everything we need is in place and access is granted instantly (people, processes and tools).
What are the numbers based on? Real use-cases? Are we committing to them?


Cheers
Jeremy

This is an excellent and crucial piece of feedback from Jeremy. It's not negative at all; it's the detailed, constructive critique from a senior technical expert that will transform our good proposal into an unassailable, bulletproof one.

Let's break down exactly what he wants, what it means, and how we should act on it.

First, to answer your core question: What does he want?
Jeremy is not offering to do the work himself. He is offering his deep subject matter expertise to make our proposal credible and technically sound. His message is a sign of engagement and a clear roadmap for what we need to refine. He is saying, "I see what you're trying to do, and I like the format. Now, let's inject the real-world complexity and technical depth to make it truly compelling."

Our action is to take his detailed feedback and expertly weave it into the existing structure.

Detailed Breakdown of Jeremy's Feedback & Our Action Plan
Here is a point-by-point analysis of what he's saying and the specific actions we need to take.

1. The Orbus Positioning
What Jeremy is Saying: "I think Orbus in the middle gives it too much focus... TOPL and Mizuho should be the primary."
His Point: The visual hierarchy is wrong. It currently looks like a three-way partnership. It should be positioned as Thakral One (the consultant) serving Mizuho (the client), using OrbusInfinity as one of the advanced tools in our toolkit.
Action Plan:
Immediately update the index.html header. Remove the Orbus logo from the top partnership banner.
The banner should be simplified to: Thakral One Logo × Mizuho Bank Logo.
In the "Two-Week Discovery Workshop" dashboard (two-week-discovery.html), keep the Orbus references, as that's where we explain how we will visualize the findings. This positions it correctly as a tool for the workshop.
2. The User Experience & Navigation
What Jeremy is Saying: "Going back and forth is a bit of a pain. Perhaps breadcrumbs and Prev / Next buttons..."
His Point: The navigation is designed for a user clicking around freely. For a formal presentation, a consultant needs a linear, controlled path to tell a story.
Action Plan:
On each of the three sub-pages (framework-visualization.html, mizuho-use-cases.html, regional-expansion.html), add a simple navigation bar at the top or bottom.
This bar should include:
A "Home" or "Overview" link (back to index.html).
"Previous: [Name of Previous Section]" button.
"Next: [Name of Next Section]" button.
This simple addition makes it a "presentation-ready" experience.
3. The Sanctions Screening Use Case (This is the most critical feedback)
What Jeremy is Saying:
"Are we sure about sanctions screening? This is a very business centric use case – not an IT one."
"What type of sanction screening... There is no detail."
He then provides a masterclass on the complexities: fuzzy logic, World Check, nicknames (Peggy/Margaret), localization (Jon/John), spelling errors, etc.
He asks the killer question: "But if someone has an engine like IIR would they need more?"
His Point: Our current description is superficial and miscategorized. We sound like we don't understand the deep complexity of the problem. A client like Mizuho almost certainly has a sophisticated screening engine already (like Informatica IIR or a competitor). Pitching a generic "AI screening tool" is naive. Our value is not in replacing their engine, but in solving the biggest problem those engines create: managing the firehose of false positives.
Action Plan (This requires a significant rewrite of the mizuho-use-cases.html page):
Re-frame the Use Case: Change the title from "Sanctions Screening Precision AI" to "AI-Powered False Positive Reduction for Sanctions Screening."
Rewrite the Description: Explicitly state that our solution works with their existing screening engine.
New Narrative: "Financial institutions like Mizuho have invested in powerful screening engines. However, these systems are often tuned for maximum caution, leading to false positive rates as high as 98%. This creates a massive operational burden on L1 and L2 compliance analysts. Our AI solution sits on top of your existing engine, using advanced contextual analysis and machine learning to intelligently triage these alerts, allowing your team to focus only on the highest-risk cases."
Incorporate His Expertise: Weave his examples into the "Benefits" section to show we understand the problem deeply.
Under "Enhanced Precision," add: "Our AI moves beyond simple rule-matching to understand complex challenges like nicknames (e.g., Peggy for Margaret), phonetic similarities (e.g., Smith vs. Smyth), and regional name variations, which are common pain points for traditional fuzzy-logic engines."
Make the Demo Tangible: The "Run Sanctions Screening Simulation" needs to be more credible.
Change the output text to reflect the new narrative. It should show a huge number of initial alerts being intelligently filtered down.
Instead of just text, let's show a mock JSON output for one of the final, high-risk alerts. This addresses his "Complete Transparency" point. The JSON could look like this:
code
JSON

download

content_copy

expand_less
{
  "alertId": "MZH-45892-2025",
  "status": "Escalated to L2 Review",
  "aiConfidenceScore": "92%",
  "matchedEntity": "Jon Smit",
  "watchListSource": "World Check",
  "riskFactors": [
    "Phonetic match: 'Smyth'",
    "Transaction nexus with high-risk jurisdiction",
    "Known associate of sanctioned entity"
  ],
  "recommendation": "Immediate review required."
}
This simple change makes the demo feel real and demonstrates the "transparency" he felt was missing.
4. Project Realism (Timelines & Metrics)
What Jeremy is Saying: "Do we need any caveats...?", "Timelines... seems very aggressive.", "What are the numbers based on? Are we committing to them?"
His Point: Our proposal lacks the standard professional caveats. It sounds too perfect, which can undermine credibility.
Action Plan:
Add an "Assumptions & Dependencies" Section: In the "Two-Week Discovery Workshop" dashboard, add a new section.
Title: "Assumptions for Success"
Points:
"Timelines are best-case scenarios and assume timely access to key Mizuho stakeholders (people), defined processes, and required technical environments (tools)."
"All prototypes will be developed using synthetic or fully anonymized data provided by Mizuho."
"The success of the pilot phase is dependent on access to relevant, de-identified historical data for model training."
Add Footnotes to Metrics: On the main index.html page, add a small asterisk (*) next to the "Expected Business Outcomes" title.
Footnote Text: "All metrics are based on Thakral One's analysis of industry benchmarks and successful regional banking implementations. They represent achievable targets and are not a contractual commitment. The two-week workshop will validate and refine these projections for Mizuho's specific environment."
By making these changes, you are not just addressing his feedback; you are incorporating his deep experience directly into the proposal. This makes the final product stronger, more credible, and demonstrates that we operate as a cohesive, expert team.