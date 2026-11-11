# Release Checklist

Quarter-end (Q4) release readiness checklist.

## Pre-release

- [ ] All tests green on the release branch (unit, integration, E2E)
- [ ] Release notes drafted and reviewed
- [ ]ogo version bumped in `package.json` / `VERSION` file
- [ ] Feature flags for the release are designed and documented

## Release sign-off

- [ ] Product owner signs off on scope and acceptance criteria
- [ ] Engineering lead confirms no open blockers
- [ ] Support team briefed on known issues and talking points

## Customer comms

- [ ] Release announcement sent to customers and partners
- [ ] In-product release note banner published
- [ ] Customer support runbook updated with rollback guidance

## Metrics dashboard

- [ ] Release readiness dashboard updated with go/no-go decision
- [ ] Success metrics defined (error rate, latency p95, adoption)
- [ ] On-call rotation confirmed for the release window

## Final

- [ ] Rollback plan reviewed and rollback owner on call
- [ ] Pre-release smoke test passed in staging
- [ ] Release cut and published
