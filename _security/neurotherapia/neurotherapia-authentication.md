---
api_key_in: []
auth_types:
- none
- bearer-visitor-token
description: ''
kind: authentication
layout: security
method: probed
name: Neurotherapia Authentication
name_suffix: Authentication
oauth_flows: []
overview: NeuroTherapia secures its APIs with none and bearer-visitor-token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NeuroTherapia
provider_slug: neurotherapia
scheme_count: 2
schemes:
- applies_to: MCP transport, tools/list, GetBusinessDetails, SearchInSite, SearchSiteApiDocs, BrowseWixRESTDocsMenu, ReadFullDocsArticle, ReadFullDocsMethodSchema
  evidence: POST tools/list with no Authorization header returned HTTP 200 and the full nine-tool list on 2026-08-26. The provider's own llms.txt states "No authentication required to connect to the MCP endpoint".
  name: anonymous
  sources:
  - https://www.neurotherapia.com/_api/mcp
  - https://www.neurotherapia.com/llms.txt
  type: none
- applies_to: CallWixSiteAPI, ExecuteWixAPI
  evidence: Both write-capable tools declare visitorToken in their required[] inputSchema; the GenerateVisitorToken tool description states it must be called first to obtain the token. The token is issued anonymously — no account, key or consent step is involved.
  in: tool-argument
  minted_by: GenerateVisitorToken
  name: visitorToken
  parameter: visitorToken
  scheme: opaque-session-token
  sources:
  - mcp/neurotherapia-mcp-tools.json
  type: bearer
slug: neurotherapia-authentication
source_filename: neurotherapia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: https://www.neurotherapia.com/_api/mcp\nnote: '0-working/derive-authentication.py returned no profile because this provider publishes no OpenAPI\n  or Swagger document. This profile is transcribed instead from a live, unauthenticated probe of the only\n  machine-readable surface the company serves — the Wix-provisioned site MCP endpoint on its own host —\n  and from the tool inputSchemas saved verbatim at mcp/neurotherapia-mcp-tools.json.'\nsummary:\n  types: [none, bearer-visitor-token]\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_connect: true\n  registration_required: false\nschemes:\n- name: anonymous\n  type: none\n  applies_to: MCP transport, tools/list, GetBusinessDetails, SearchInSite, SearchSiteApiDocs,\n    BrowseWixRESTDocsMenu, ReadFullDocsArticle, ReadFullDocsMethodSchema\n  evidence: 'POST tools/list with no Authorization header returned HTTP 200 and the full nine-tool list\n    on 2026-08-26. The provider''s\
  \ own llms.txt states \"No authentication required to connect to the MCP\n    endpoint\".'\n  sources: [https://www.neurotherapia.com/_api/mcp, https://www.neurotherapia.com/llms.txt]\n- name: visitorToken\n  type: bearer\n  scheme: opaque-session-token\n  in: tool-argument\n  parameter: visitorToken\n  applies_to: CallWixSiteAPI, ExecuteWixAPI\n  minted_by: GenerateVisitorToken\n  evidence: 'Both write-capable tools declare visitorToken in their required[] inputSchema; the\n    GenerateVisitorToken tool description states it must be called first to obtain the token. The token\n    is issued anonymously — no account, key or consent step is involved.'\n  sources: [mcp/neurotherapia-mcp-tools.json]\noauth2:\n  present: false\n  evidence: '/.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource both\n    returned HTTP 400 on 2026-08-26; the MCP endpoint issued no OAuth challenge on an anonymous\n    tools/list.'\nabsent:\n- api_keys\n- oauth2\n- openid_connect\n\
  - mutual_tls\n- signed_requests\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neurotherapia/refs/heads/main/authentication/neurotherapia-authentication.yml
summary_line: none/bearer-visitor-token · 2 schemes
tags:
- Biotechnology
- Pharmaceuticals
- Life Sciences
- Health
- Clinical Trials
- Neuroscience
- Drug Discovery
- Alzheimers Disease
- Company
---
