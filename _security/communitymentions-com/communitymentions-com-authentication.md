---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: CommunityMentions Authentication
name_suffix: Authentication
oauth_flows: []
overview: CommunityMentions declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CommunityMentions
provider_slug: communitymentions-com
scheme_count: 1
schemes:
- description: The MCP endpoint (advertised as "Official access" on communitymentions.com) answered a JSON-RPC tools/list with HTTP 200 and two tools (find_subreddits, get_subreddit) without any credential; no WWW-Authenticate header was returned.
  endpoint: https://communitymentions.com/api/mcp
  http_status: 200
  type: none
slug: communitymentions-com-authentication
source_filename: communitymentions-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://communitymentions.com/api/mcp\nschemes:\n- type: none\n  description: The MCP endpoint (advertised as \"Official access\" on communitymentions.com) answered a JSON-RPC tools/list with HTTP 200 and two tools (find_subreddits, get_subreddit) without any credential; no WWW-Authenticate header was returned.\n  endpoint: https://communitymentions.com/api/mcp\n  http_status: 200\nnote: No OpenAPI and no developer docs are published, so no API key, OAuth or token scheme is documented.\n"
source_yaml_url: https://artifacts.apis.io/communitymentions-com/authentication/communitymentions-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Reddit Marketing
- Brand Mentions
- Social Media Marketing
- AI Search Visibility
- Community Marketing
- SEO
- MCP
---
