---
title: "Code Reviews"
date: 2018-03-06T00:00:00-04:00
weight: 4
subsection: Getting Started
---

All changes to the product must be reviewed.

* User experience changes must be reviewed by a [product manager](/contribute/getting-started/core-committers/#product-managers).
* Code changes must be reviewed by at least two [core committers](http://localhost:1313/contribute/getting-started/core-committers/#core-committers).
* Documentation changes should be reviewed by a [product manager](/contribute/getting-started/core-committers/#product-managers) and at least one [core committer](/contribute/getting-started/core-committers/#core-committers).

If you are not a core committer
-------------------------------

1. Submit your pull request.
2. Reach out to the author of the ticket your PR resolves.
    * Typically this means [mentioning](https://help.github.com/en/articles/basic-writing-and-formatting-syntax#mentioning-people-and-teams) their username as a comment on the pull request.
    * Product managers and core committers are often on the lookout for new PRs, and may handle this for you automatically.
    * When in doubt, ask for help in the [Developers](https://community.mattermost.com/core/channels/developers) channel on our community server.
3. Wait for a review.
    * The ticket author, another core committer or a product manager will assign reviewers and label your pull request appropriately.
    * Expect some interaction with at least one reviewer within 5 business days.
    * Keep in mind that Mattermost Core Committers are geographically distributed around the world and likely in a different time zone than your own.
4. Make any necessary changes.
    * If a reviewer requests changes, your pull request will disappear from their queue of reviews.
    * Once you've addressed the concerns, reach out with another mention or via our community server.
5. Wait for your code to be merged.
    * Once all reviewers have approved your changes, they will handle merging your code.

If you are a core committer seeking a review
--------------------------------------------

1. Submit your pull request.
2. Assign a [product manager](/contribute/getting-started/core-committers/#product-managers) to your review and label your pull request with `1: PM Review`.
    * If your changes do not affect the user experience, you may skip this step.
    * Wait for their review before continuing, to avoid churn if changes are requested.
3. Assign two [core committers](/contribute/getting-started/core-committers/) to your review and label your pull request with `2: Dev Review`.
    * When picking your first core committer, consider someone with domain expertise relative to your changes. Sometimes GitHub will recommend a recent editor of the code, but often you must rely on your own intuition from past interactions.
    * When picking your second core committer, consider someone unrelated to your changes. A fresh and unbiased set of eyes can be invaluable, and exposing the team to new parts of the code helps spread out domain knowledge.
    * Don't be afraid to pick someone who gives "hard" reviews. Code review feedback is never a personal attack: it should "sharpen" the skills of both the author and the reviewers, not to mention improving the quality of the product.
    * Take into account the timeoff calendar.
    * Try to avoid assigning the same person to all of your reviews unless they are related.
    * When in doubt, ask for recommendations on our community server.
4. Wait for a review.
    * Expect some interaction with each of your reviewers within 2 business days.
    * There is no need to explicitly mention them on the pull request, or to explicitly reach out on our community server.
    * Core committers are expected to have the GitHub plugin installed to automate notifications, and to trigger a daily review of their outstanding requested reviews.
5. Make any necessary changes.
    * If a reviewer requests changes, your pull request will disappear from their queue of reviews.
    * Once you've addressed the concerns, assign them as a reviewer again to put your pull request back on their plate.
6. Once all concerns have been addressed, a product manager has approved the changes (as necessary), and at least two core committers have approved, the pull request is ready to be merged.
    * Remove the `1: PM Review` and `2: Dev Revew` labels and assign the `3: Ready to Merge` label.
    * Merge your pull request, and delete the branch if not from a fork.
    * Note that the last core committer to approve your changes may do this on your behalf.
    * If your pull request depends on other pull requests, consider assigning the `Awaiting PR` label.

If you are a core committer asked to give a review
--------------------------------------------------

1. Respond quickly to requested reviews.
    * Assume the requested review is urgent and blocking unless explicitly stated otherwise.
    * Try to interact with the author within 2 business days.
    * Configure the GitHub plugin to automate notifications.
    * Review your outstanding requested reviews daily to avoid blocking authors.
    * Responding quickly doesn't necessarily mean reviewing quickly! Just don't leave the author hanging.
2. Feel free to clarify expectations with the author.
    * If the code is experimental, they may need only a cursory glance and thumbs up to proceed with productizing their changes.
    * If the review is large or complex, additional time may be required to complete your review. Be upfront with the author.
    * If you are not comfortable reviewing the code, avoid "rubber stamping" the review. Be honest with the author and ask them to consider another core committer.
3. Never rush a review.
    * Take the time necessary to review the code thoroughly.
    * Don't be afraid to ask for changes repeatedly until all concerns are addressed.
    * Feel free to challenge assumptions and timelines. Rushing a change into a patch release may cause more harm than good.
4. Merge the pull request.
    * Remove the `1: PM Review` and `2: Dev Revew` labels and assign the `3: Ready to Merge` label.
    * Merge the pull request, and delete the branch if not from a fork.
    * Some changes are spread out across multiple PRs that should be merged at the same time. Look out for the `Awaiting PR` label. When in doubt, leave the merging the pull request to the author.