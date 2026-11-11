# Rollback Plan

Step-by-step recovery procedure for a bad release.

## Rollback owner

- Rollback owner: On-call release engineer (see `#release-oncall` in Slack)
- Backup reviewer: Release manager

## Steps

1. **Declare incident** — notify the queue in `#release-incidents` and start a war room.
2. **Freeze the deployment** — if automated canary is enabled, keep it from rolling forward.
3. **Revert the release commit** — redeploy the previous tagged release from the artifact store.
4. **Verify the revert** — confirm the version on every environment matches the last known-good tag.
5. **Communicate** — post an update in `#release-incidents` with the root cause and next steps.
6. **Post-mortem** — write a blameless post-mortem within 48 hours and attach it to the release issue.

## Contacts

- On-call release engineer: PagerDuty rotation `release-oncall`
- Release manager: release-manager@internal
- escalation: ping `#release-oncall` in GitHub then page the release manager
