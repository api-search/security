---
api_key_in: []
auth_types: []
description: 'Authentication profile for Lindy. Derived from documentation rather than a spec, because Lindy publishes no OpenAPI securitySchemes. Two distinct directions must not be confused: how a caller authenticates TO Lindy (one scheme, on one endpoint), and how Lindy authenticates OUT to the tools it integrates with (OAuth and API keys, the much larger surface).'
kind: authentication
layout: security
method: searched
name: Lindy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lindy declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Lindy
provider_slug: lindy
scheme_count: 0
schemes: []
slug: lindy-authentication
source_filename: lindy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://docs.lindy.ai/skills/by-lindy/webhooks ,\n  https://docs.lindy.ai/integrations/credentials ,\n  https://docs.lindy.ai/integrations/mcp , live probes\nprovider: Lindy\nproviderId: lindy\ndescription: >-\n  Authentication profile for Lindy. Derived from documentation rather than a\n  spec, because Lindy publishes no OpenAPI securitySchemes. Two distinct\n  directions must not be confused: how a caller authenticates TO Lindy (one\n  scheme, on one endpoint), and how Lindy authenticates OUT to the tools it\n  integrates with (OAuth and API keys, the much larger surface).\nderived_from_spec: false\nspec_reason: No OpenAPI is published. See conformance/lindy-conformance.yml.\ninbound:\n  description: How an external caller authenticates to a Lindy-hosted endpoint.\n  schemes:\n    - id: webhook-bearer\n      type: http\n      scheme: bearer\n      applies_to: https://public.lindy.ai/api/v1/webhooks/[unique-id]\n   \
  \   header: 'Authorization: Bearer [your-secret-key]'\n      credential: >-\n        A per-webhook secret generated in the Lindy UI and displayed exactly\n        once. No prefix convention, expiry, rotation procedure or revocation\n        endpoint is documented.\n      scoped: per webhook\n      source: https://docs.lindy.ai/skills/by-lindy/webhooks\n    - id: mcp-anonymous\n      type: none\n      applies_to: https://docs.lindy.ai/mcp\n      detail: >-\n        The documentation MCP server accepts anonymous calls;\n        /.well-known/mcp.json declares \"authentication\": \"none\". Verified by an\n        unauthenticated tools/list returning 200 on 2026-08-29.\n      source: https://docs.lindy.ai/.well-known/mcp.json\noutbound:\n  description: >-\n    How Lindy authenticates to third-party tools on the user's behalf. This is\n    the dominant auth surface in Lindy's docs, and it is Lindy acting as client.\n  models:\n    - id: oauth-connect\n      type: oauth2\n      detail: >-\n \
  \       Most integrations connect with an OAuth button; every action for that\n        tool is enabled at once. Multiple accounts can be attached to one\n        integration.\n      source: https://docs.lindy.ai/integrations/overview\n    - id: stored-credential\n      type: apiKey\n      detail: >-\n        Tools without an OAuth flow use a saved credential — an API key stored\n        once in the workspace, named for the tool (e.g. NOTION_API_KEY), kept\n        private or shared with the workspace, and used by Lindy without being\n        pasted into a chat.\n      source: https://docs.lindy.ai/integrations/credentials\n    - id: mcp-server-auth\n      type: mixed\n      detail: >-\n        For third-party MCP servers Lindy connects to: anonymous and\n        OAuth-flow servers need nothing configured; a static credential can be\n        sent as an Authorization bearer token, a custom header, or a query\n        parameter.\n      source: https://docs.lindy.ai/integrations/mcp\nenterprise_identity:\n\
  \  sso: 'Listed as an Enterprise-tier feature on https://docs.lindy.ai/pricing'\n  scim: 'Listed as an Enterprise-tier feature on https://docs.lindy.ai/pricing'\n  documented_configuration: false\noauth_server:\n  published: false\n  probes:\n    - url: https://www.lindy.ai/.well-known/oauth-authorization-server\n      status: 404\n    - url: https://docs.lindy.ai/.well-known/oauth-authorization-server\n      status: 404\n    - url: https://docs.lindy.ai/.well-known/oauth-protected-resource\n      status: 404\n    - url: https://www.lindy.ai/.well-known/openid-configuration\n      status: 404\nscopes:\n  published: false\n  note: >-\n    No OAuth scope reference exists for Lindy as a provider — Lindy issues no\n    OAuth tokens. scopes/ is therefore deliberately not written; see the\n    OAuth-only applicability rule in pipeline-enrich.md.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lindy/refs/heads/main/authentication/lindy-authentication.yml
summary_line: 0 schemes
tags:
- AI Agents
- AI Automation
- Agentic AI
- MCP
- Workflow-Automation
- Virtual Assistant
- Productivity
- Email
- Meetings
- Slack
---
