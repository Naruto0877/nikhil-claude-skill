# Nikhil Claude Skill

Use this workflow for Nikhil's coding tasks. Match the effort to the change: a typo fix needs a quick check; a behavioral change needs evidence that the behavior works.

## 1. Understand the goal and act

- Read relevant project instructions and trace the existing implementation before editing.
- Turn the request into an observable outcome. For a bug, identify the failing behavior; for a feature, identify how the user will use it.
- Make routine implementation choices from project conventions. State consequential assumptions briefly and continue useful work.
- Ask a focused question when missing information materially changes the product, public API, data handling, or cost. Avoid repeating questions already answered in the conversation.
- Carry an authorized action request through implementation and verification. A plan or explanation alone does not complete an implementation request.

## 2. Choose the simplest implementation

- Reuse the project's existing components and patterns before introducing dependencies or abstractions.
- Implement the requested behavior without speculative features, configuration, or extensibility.
- Keep functions and interfaces easy to follow. Prefer a small direct solution over a framework built for a single use.
- Preserve error handling at real failure boundaries; do not remove safeguards just to shorten the code.

## 3. Keep the change focused

- Match the surrounding code style and preserve unrelated edits and behavior.
- Change adjacent code only when necessary for the requested outcome. Mention unrelated problems separately.
- Remove imports, variables, and helpers made unused by this change. Leave unrelated cleanup for a separate request.
- Review the final diff: each changed line should support the requested outcome or its verification.

## 4. Verify and finish

- Choose checks that demonstrate the result. Reproduce a bug before fixing it when practical; add a regression test when it protects meaningful behavior.
- Run the relevant tests, build, lint, or manual check for the affected area. A documentation-only or trivial visual edit does not require an invented test suite.
- Broaden checks when a failure, shared dependency, or unresolved concern justifies it. Once appropriate checks pass, finish instead of repeatedly running the same checks.
- Distinguish verified results from assumptions. If a check cannot run, explain the concrete blocker and what remains unverified.
- Existing task authorization applies throughout the work. Publishing, deployment, and other external actions still require the authorization appropriate to that action.

## Work efficiently and communicate clearly

- Search for relevant symbols and files before reading entire directories. Batch independent reads and inspect their results; keep dependent edits sequential.
- Use tools and reusable project scripts where they reduce repeated work. Avoid broad scans, repeated reads, or retries without new evidence.
- Give short progress updates when findings or decisions change the work. Finish with what changed, how it was checked, and any remaining limitation.

Adapted for Nikhil from [andrej-karpathy-skills](https://github.com/multica-ai/andrej-karpathy-skills), inspired by Andrej Karpathy's observations on coding agents. Original skill declares the MIT license.
