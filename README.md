# Desert Road Catholic MCP server

A free, public [Model Context Protocol](https://modelcontextprotocol.io) server for
[Desert Road Catholic](https://desertroadcatholic.com), an independent, unofficial daily companion for
Catholic men doing Exodus 90 in 2027 (Day 1 is Monday, January 11, 2027; Day 90 is Saturday, April 10, 2027).

- **Endpoint:** `https://desertroadcatholic.com/mcp`
- **Transport:** Streamable HTTP (stateless JSON-RPC over POST)
- **Authentication:** none
- **Cost:** free

## Tools

| Tool | What it does |
|---|---|
| `get_program_info` | Overview of the program, dates, cost and links. |
| `get_day` | The reading, stage and opening prayer for a day number (1-90) or a date. Defaults to today (America/New_York). |
| `list_stages` | The six stages and the 90 Douay-Rheims readings grouped by stage. |
| `get_prayer` | The text of a stage opening prayer, the Te Deum, or a hard-day prayer. |
| `register` | Registers a man for the free welcome emails. Requires `email` and `user_confirmed: true`; optional `first_name` and `leader`. |

Scripture is the Douay-Rheims (Challoner) translation.

## Using it

Add `https://desertroadcatholic.com/mcp` as a remote MCP server (custom connector) in your MCP client.
No API key is needed. Registration only happens when the user has confirmed they want it.

## Registry

Published to the official MCP Registry as `com.desertroadcatholic/desert-road-catholic`.

## Independence

Desert Road Catholic is an independent, unofficial companion. It is not affiliated with, endorsed by, or
connected to Exodus 90 or its publishers.

## License

[MIT](LICENSE) for the contents of this repository.
