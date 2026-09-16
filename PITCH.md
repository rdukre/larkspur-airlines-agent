# PITCH.md

Six lines and a lever. Your words. The last two are scored.

Built:
AI-powered Larkspur Airlines disruption support agent connected to booking, flight status, policy, rebooking, escalation, and MCP-hosted tools.

Does:
Helps disrupted passengers understand options, find travel alternatives, check policies, and determine the earliest available travel date through natural language conversations.

Number:
Passed all Build 1 and Build 2 verification gates, including successful routing and execution of next_available_day through MCP.

Guardrail:
Requires customer confirmation before irreversible booking actions and escalates out-of-scope requests to a human agent.

Next:
Expand evaluation coverage, add more operational scenarios, and improve production-readiness through broader testing.

Still broken:
Limited scenario coverage, no advanced inventory optimization, no refund automation, and additional real-world testing is still required.

Lever: intelligence

## Priya asked

Costs:
11 tools currently add approximately 1,329 schema tokens to every model turn; MCP improves ownership and reuse but does not reduce schema token cost by itself.

Wrong:
The agent can still be wrong if source tools, policies, or operational data are incomplete or inaccurate, and broader evaluation coverage is still needed.

Runs it:
Claude Sonnet 5 orchestrates tool calls, with airline capabilities provided through local tools and MCP-hosted services.
