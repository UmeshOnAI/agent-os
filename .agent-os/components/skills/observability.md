# Observability Skill

Application logs must be structured single-line JSON containing at least:
timestamp, level, service, correlation_id, event_code, context.

Every inbound request, background job, and outward API call must propagate correlation_id.

Agents must be able to isolate end-to-end failure traces via jq or equivalent without ingesting raw log dumps.