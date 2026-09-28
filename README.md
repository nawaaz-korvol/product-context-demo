# Product context, with a memory

A small example of keeping product context useful to people and agents as decisions change.

**Everything in this example is fictional.** Research, priorities, and product decisions are teaching fixtures, not company information or evidence of a shipped product. There is no application here.

## The two-minute tour

A team starts with a broad document-onboarding idea. New observations suggest a smaller pilot. How does everyone catch up without rereading every conversation?

1. Read the [current initiative](initiatives/document-collection.md): direction, scope, and unanswered questions.
2. Follow its [decision record](decisions/001-initial-direction.md) to the [source material](research/001-initial-intake.md).
3. Skim the [changelog](CHANGELOG.md) to see what changed.
4. Open the [sample scope-change PR](https://github.com/nawaaz-korvol/product-context-demo/pulls): research, decision, brief, and changelog move together.

`main` is the accepted **demo baseline**. An open PR is a proposal, even when an agent wrote it confidently. Merging a document change accepts direction; it does not mean the product has been built, tested, or released.

## A small convention

| Question | Authority |
|---|---|
| What is our current direction? | Initiative brief on `main` |
| Why that direction? | Dated decision records and linked evidence |
| What changed? | Append-only changelog |
| What is assigned, in progress, or done? | Linked tracker issue |

Use [agent instructions](AGENTS.md) and the [PR template](.github/pull_request_template.md) to keep those boundaries clear. Log changes to scope, assumptions, decisions, or outcomes; skip typo-only updates. Keep raw evidence distinguishable from interpretation.

This demo uses GitHub Issues as a stand-in for a team's task tracker. There is no Linear or ClickUp integration. A local checkout only reflects the last fetched version; refresh it before treating it as current.
