# Incident Response

## When to Use

A production service is degraded or unavailable.

## Severity Levels

| Level | Description | Response Time |
|-------|-------------|---------------|
| SEV-1 | Complete outage, all users affected | Immediate |
| SEV-2 | Major feature broken, many users affected | < 30 minutes |
| SEV-3 | Minor issue, workaround available | < 4 hours |

## Steps

1. **Acknowledge** — confirm the incident in the team channel.
2. **Assess** — determine severity and affected services.
3. **Communicate** — notify stakeholders based on severity.
4. **Investigate** — check logs, metrics, and recent deployments.
5. **Mitigate** — apply a fix or rollback.
6. **Verify** — confirm the service is healthy.
7. **Post-mortem** — schedule a blameless review within 48 hours.

## Escalation

If the issue is not resolved within the expected response time, escalate to the engineering lead.

## Useful Commands

```bash
# Check service health
curl http://localhost:7007/healthcheck

# View recent logs
docker logs <container-name> --tail 100

# Restart a service
docker restart <container-name>
```
