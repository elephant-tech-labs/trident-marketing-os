# Client Type Rules

Current field:
`Client type`

Allowed values:
- Agent
- Homeowner

## Rules

If `Client type = Agent`, route only to agent workflows.

If `Client type = Homeowner`, route only to homeowner workflows.

## Future Improvement

A contact can be both a homeowner and an agent. Eventually, replace single picklist with:
- Client Roles multi-select
- Related service/relationship records
