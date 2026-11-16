# AI workflow case study: long-running engineering work

I’m Austin Purdy, a Navy veteran with an electrical and engineering background. I direct AI-assisted development on a long-running personal software project. My focus is keeping work moving across sessions while protecting existing functionality and checking what the system actually does.

## The challenge

AI assistants can lose context, repeat work, or treat a proposal as a finished result. On a project that evolves over many sessions, I need a way to keep decisions accessible, coordinate work, and know when a change is ready for use.

## How I work

- **Keep context usable:** maintain current instructions, ownership boundaries and handoffs so an agent can find the relevant material without treating every old report as current.
- **Direct and challenge the work:** set the desired outcome and constraints, delegate bounded tasks, question unnecessary work, and use judgment to balance product quality with forward progress.
- **Protect the working product:** develop candidates separately, preserve an accepted version, and promote changes only when the relevant evidence supports the decision.
- **Separate claims from evidence:** distinguish what is intended, implemented, checked or measured, and record limitations rather than presenting a local test as production performance.

## Example: containing a failure

In one AI-assisted investigation, a malformed saved record could cause a shared service to stop, affecting other users. The work explored a more contained response: refuse the affected record without changing it while allowing other users to continue.

The project report describes a local comparison against the earlier implementation: it exercised several invalid records, checked that rejected data stayed unchanged, and observed another test client continuing to operate. It also identified limits: some branches were not exercised, a related client change had not been compiled, and installation integration was still pending in that report. These are development results, not evidence of production deployment or capacity.

My role is directing the work, establishing priorities and constraints, reviewing AI-produced findings, and deciding what to pursue. AI agents contribute research, implementation, and testing under that direction. The underlying project remains private; this example is described at a level intended to demonstrate the workflow without publishing its source or proprietary design.

## Read the paper

[Dynamic Rules for Long-Horizon Work on Static AI (PDF)](./Dynamic%20Rules%20for%20Long-Horizon%20Work%20on%20Static%20AI.pdf)

The paper describes the approach as a practitioner case study. It is not a controlled benchmark or a claim that the workflow eliminates AI errors.
