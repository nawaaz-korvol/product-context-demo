# Product context, with a memory

A small example of keeping product context useful to people and agents as decisions change.

**Everything in this example is fictional.** Research, priorities, and product decisions are teaching fixtures, not company information or evidence of a shipped product. There is no application here.

This example demonstrates shared context and decision history. It does not yet cover technical requirements, architecture, roadmaps, task delegation, or feeding implementation outcomes back into the documents.

## The two-minute tour

A team starts with a broad document-onboarding idea. New observations suggest a smaller pilot. How does everyone catch up without rereading every conversation?

1. Read the [current initiative](initiatives/document-collection.md): direction, scope, and unanswered questions.
2. Follow the decision and evidence links in that brief to understand its rationale.
3. Skim the [changelog](CHANGELOG.md) to see what changed.
4. Open the [sample scope-change PR](https://github.com/nawaaz-korvol/product-context-demo/pull/2): research, decision, brief, and changelog move together.

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

## Try the reader check

Give a fresh reader or agent the repo and ask: What is accepted? What is proposed? What evidence supports it? What is still undecided? Where is delivery status, and has anything shipped?

**Run on 2026-09-28:** two separate agent readers inspected the baseline and the scope-change proposal. Both answered all five questions consistently with the documents. The proposal reader correctly distinguished the broader accepted direction from the narrower proposal, identified the synthetic evidence and counterexample, and did not mistake acceptance for delivery. Relative Markdown links were also checked with a local script.

This is a comprehension check, not proof of team adoption or product value. The readers used local files and Git refs; live GitHub state was checked separately during publication. A useful next trial is to have a teammate make a second change and see whether another reader can reconstruct it without explanation.
