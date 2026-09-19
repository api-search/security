---
anonymous_access: true
api_key_in: []
auth_types: []
description: 'Agragene publishes no REST/GraphQL API and therefore no securitySchemes. The only callable surface is the site MCP endpoint, which is ANONYMOUS: an unauthenticated JSON-RPC initialize and tools/list both returned HTTP 200 on 2026-09-12, and the company''s own llms.txt states "No authentication required to connect to the MCP endpoint". A per-session visitor token exists one level down, minted by the GenerateVisitorToken tool and required only as an argument to CallWixSiteAPI / ExecuteWixAPI; it is not a credential a consumer registers for.'
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Agragene Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agragene declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Agragene
provider_slug: agragene
scheme_count: 2
schemes:
- applies_to: https://www.agragene.com/_api/mcp
  evidence:
    http_status: 200
    method: POST tools/list (no Authorization header)
    url: https://www.agragene.com/_api/mcp
  id: mcp-anonymous
  note: Connection and tool enumeration require no credential of any kind.
  transport: http-jsonrpc
  type: none
- applies_to: CallWixSiteAPI, ExecuteWixAPI
  evidence:
    quote: GenerateVisitorToken - Creates a new visitor session and obtains a visitor access token for the site. Must be called before making any CallWixSiteAPI request.
    url: https://www.agragene.com/llms.txt
  id: wix-visitor-token
  issued_by: GenerateVisitorToken (MCP tool, no parameters)
  note: Platform-minted anonymous session token, not a provider-issued API key. Scope is limited to public site information; no Wix business solution is installed on this site, so no transactional data is reachable with it.
  registration_required: false
  type: bearer-session
slug: agragene-authentication
source_filename: agragene-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://www.agragene.com/_api/mcp\ndocs: https://www.agragene.com/llms.txt\ndescription: >-\n  Agragene publishes no REST/GraphQL API and therefore no securitySchemes. The only\n  callable surface is the site MCP endpoint, which is ANONYMOUS: an unauthenticated\n  JSON-RPC initialize and tools/list both returned HTTP 200 on 2026-09-12, and the\n  company's own llms.txt states \"No authentication required to connect to the MCP\n  endpoint\". A per-session visitor token exists one level down, minted by the\n  GenerateVisitorToken tool and required only as an argument to CallWixSiteAPI /\n  ExecuteWixAPI; it is not a credential a consumer registers for.\nschemes:\n- id: mcp-anonymous\n  type: none\n  applies_to: https://www.agragene.com/_api/mcp\n  transport: http-jsonrpc\n  evidence:\n    url: https://www.agragene.com/_api/mcp\n    method: POST tools/list (no Authorization header)\n    http_status: 200\n  note: Connection and tool\
  \ enumeration require no credential of any kind.\n- id: wix-visitor-token\n  type: bearer-session\n  applies_to: CallWixSiteAPI, ExecuteWixAPI\n  issued_by: GenerateVisitorToken (MCP tool, no parameters)\n  registration_required: false\n  evidence:\n    url: https://www.agragene.com/llms.txt\n    quote: >-\n      GenerateVisitorToken - Creates a new visitor session and obtains a visitor access\n      token for the site. Must be called before making any CallWixSiteAPI request.\n  note: >-\n    Platform-minted anonymous session token, not a provider-issued API key. Scope is\n    limited to public site information; no Wix business solution is installed on this\n    site, so no transactional data is reachable with it.\noauth: false\napi_keys: false\nmutual_tls: false\nopenid_connect: false\nnotes:\n- No /.well-known/oauth-protected-resource or /.well-known/oauth-authorization-server is served (HTTP 400 on both).\n- No developer portal, signup, or key-provisioning flow exists on any Agragene\
  \ host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agragene/refs/heads/main/authentication/agragene-authentication.yml
summary_line: 2 schemes
tags:
- Agriculture
- AgTech
- Biotechnology
- Gene Editing
- Pest Control
- Sustainability
- Food and Beverage
- Life Sciences
- Company
---
