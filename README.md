# Iridium - LinkedIn MCP for AI Agents

[![Iridium on Peerlist](https://peerlist.io/api/v1/projects/embed/PRJH7B8E7Q89LRMMJFR8BAQPMMJ7J9?showUpvote=true&theme=dark)](https://peerlist.io/macandpc/project/iridium--linkedin-for-ai-agents)

MCP server connecting your AI agents (Claude, Hermes, ChatGPT, and any MCP client) to your LinkedIn context.

Your agents can complete repetitive outreach (LinkedIn connection requests, commenting on posts, handling a large number of messages) so you can focus on getting the work done. Explicit approval is needed from you before agentic actions occur.

Iridium reads live LinkedIn data through your own authorized session - no scraping.

[iridiumhqmcp.com](https://iridiumhqmcp.com)

## Who is this for

Busy professionals who are strategic with their LinkedIn outreach (hiring, building a brand, jobseeking) by giving your agent (with knowledge of your specific workflows) access to your LinkedIn environment.

1) Explicit user approval needed before agentic actions occur

2) Audit log so all agentic actions are visible to you.

3) Schedule actions on LinkedIn (connection requests, post comments)

4) Triage a full inbox - sort what came back, draft the answers, and send them at a sensible hour.

## How to add this MCP to your agent

Iridium is a hosted, remote MCP server. Add this URL to any MCP client and sign in:

    https://api.iridiumhqmcp.com/mcp

**Claude (web / desktop / mobile):** Settings → Connectors → Add custom connector → paste the URL → sign in.

**Hermes Agent:** add to `~/.hermes/config.yaml`, then restart or run `/reload-mcp`:

```yaml
mcp_servers:
  iridium:
    url: https://api.iridiumhqmcp.com/mcp
    auth: oauth
```

**Cursor / VS Code / Windsurf:** add a remote MCP server with the URL above.

**ChatGPT / Codex:** add it as a connector (ChatGPT Developer Mode / Codex MCP config).

## Example workflows

how many messages have I got from headhunter recruiters hiring for startups?

Your Agent will work with you to sort your messages based on your needs.

Help me find Engineers who have deployed voice AI systems in the past 12 months.

Your Agent has the tools to search for roles with specific filters in mind, then also plan outreach for approved candidates.

I'm building a brand selling Self Healing Agents, let's find posts talking about that to find prospective inbound.

Your Agent can help you filter posts to comment on, making your brand more visible. Schedule the comments to go out whenever.

## Star this repo

Iridium is early and built in the open. If it's useful to you, starring the repo helps other developers discover it - and tells me what to build next.
