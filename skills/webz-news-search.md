---
name: webz-news-search
description: Search global news with the Webz.io news_search_by_webz MCP tool. Use for any question about news, current events, or recent developments around a topic, company, person, or place.
api: Webz.io News Search API
operations:
  - news_search_by_webz
x-provenance:
  generated: '2026-08-27'
  method: searched
  source: https://docs.webz.io/docs/webz/news-search-api-skill
  note: >-
    Published verbatim by Webz.io on their Agent Skill documentation page. The body below is the
    provider's own skill file, copied unchanged. Only this x-provenance block was added.
---

# Webz.io News Search

Use the `news_search_by_webz` MCP tool to answer news and current-events questions.

## When to use

- The user asks about news, recent events, announcements, or coverage of a topic.
- Fresh, sourced information matters more than general knowledge.

## How to call

- `query`: a natural-language topic or question ("EU AI regulation progress"), not keyword syntax.
- The default window is the last 7 days. For older news pass `days` (up to 30) or `allow_all_dates: true`.
- `k`: articles to return - default 10, max 50. Raise it for broad research, lower it for a quick answer.

## Filters (optional, values are case-insensitive)

- `language`: full names - english, chinese, hebrew, french, spanish, german, arabic, russian, japanese, korean.
- `country`: ISO-2 uppercase codes - "US", "GB", "DE", "IL".
- `sentiment`: positive, negative, neutral.
- `domain`: include only these sources - "cnn.com", "yahoo.com".
- `exclude_domain`: skip these sources - never put the same domain in both lists.
- `category`: one of 17 values - Arts, Culture and Entertainment; Crime, Law and Justice; Disaster and Accident; Economy, Business and Finance; Education; Environment; Health; Human Interest; Labor; Lifestyle and Leisure; Politics; Religion and Belief; Science and Technology; Social Issue; Sport; War, Conflict and Unrest; Weather.

Map the user's topic to the closest category ("stock market crash" -> Economy, Business and Finance). Skip filters the user did not imply. Map source requests too: "only from BBC" -> domain: ["bbc.com"]; "ignore Yahoo" -> exclude_domain: ["yahoo.com"].

## Using results

- Each result has a title, URL, publish date, and text excerpt.
- Cite the article URLs in your answer.
- If results are empty, retry with `days: 30` or `allow_all_dates: true` and fewer filters before reporting nothing found.

## Prerequisites (from the provider's install page)

Connect the Webz.io News Search MCP server first — the MCP connection provides the tool, the skill
teaches the agent to use it well.

- Endpoint: `https://news-search-mcp.webz.io/mcp`
- Auth: `Authorization: Bearer YOUR_WEBZ_TOKEN` (the same token as the News Search API)
- Install paths documented by Webz.io: `~/.claude/skills/webz-news-search/SKILL.md` (Claude Code),
  `~/.cursor/skills/webz-news-search/SKILL.md` (Cursor)
- Every tool call is a billed News Search request: same credits, same ~1 request/second per-token
  rate limit, `402` on insufficient credits and `429` on rate-limit exhaustion.
