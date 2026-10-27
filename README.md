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
| `get_rosary_mysteries` | Which Rosary mysteries to pray on a date or weekday (defaults to today, America/New_York): the five mysteries with fruits and Douay-Rheims scripture, the weekly schedule, and a link to the free guided Rosary. Each set includes its page, markdown and pray-now URLs. |
| `list_rosary_mysteries` | All four sets of Rosary mysteries with their days, fruits and scripture, the order of prayers, and the guided Rosary link and data file. |
| `get_follow_options` | The official 2027 start date with the official page it comes from, Day 90 and Easter by our count, days until Day 1 (America/New_York), and the ways to follow along: web live now, iPhone and Android coming soon (no store links yet). |
| `register` | Registers a man for the free welcome emails. Requires `email` and `user_confirmed: true`; optional `first_name` and `leader`. |

Scripture is the Douay-Rheims (Challoner) translation.

The guided Rosary is at https://desertroadcatholic.com/armory/rosary/ (free, two-voice audio, no account). Its data, shared with the Rosary tools, is at https://desertroadcatholic.com/data/rosary.json. Each set of mysteries
has its own page, e.g. https://desertroadcatholic.com/armory/rosary/glorious-mysteries/, with a markdown twin at
`index.md` under the same path.

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
