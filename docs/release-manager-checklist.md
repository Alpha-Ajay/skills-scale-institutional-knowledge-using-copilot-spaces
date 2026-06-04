# Release Manager Checklist

Purpose: Operational checklist to reduce deployment risk and ensure consistent verification and communications.

Pre-release
- [ ] Confirm all PRs merged and passing CI
- [ ] Confirm security scans completed and critical findings addressed
- [ ] Confirm smoke & regression tests for staging passed
- [ ] Confirm rollback/mitigation plan documented
- [ ] Prepare release notes and stakeholder communications
- [ ] Schedule deployment window and notify stakeholders

Deployment
- [ ] Trigger deployment to staging (automated pipeline preferred)
- [ ] Execute staging smoke tests and sign off
- [ ] Trigger production deployment
- [ ] Monitor deployment pipeline for errors

Post-deploy
- [ ] Run post-deploy smoke tests in production
- [ ] Confirm key metrics and dashboards show expected behavior
- [ ] Announce release and provide runbook/contacts
- [ ] Capture any immediate action items and assign owners

If there is a critical failure
- [ ] Notify on-call and initiate incident response
- [ ] Rollback if mitigation plan requires it
- [ ] Triage root cause and create action items for retrospective
