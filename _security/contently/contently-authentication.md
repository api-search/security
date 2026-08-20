---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Contently Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contently secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Contently
provider_slug: contently
scheme_count: 1
schemes:
- description: 'The Contently Talent API authenticates with scoped OAuth2 access tokens. Contently states this in three places on the Talent API page: "OAuth2 with scoped tokens" (Endpoint surface), "OAuth2 with scoped tokens. Per-route rate limits. Encrypted PII." (Workspace governance), and "auth: oauth2 (scoped)" (MCP tools panel).'
  detail_note: No grant type, token endpoint, authorization endpoint, scope name, or token lifetime is published. The OAuth discovery documents that would carry them (/.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource, /.well-known/openid-configuration) return 404 on contently.com, api.contently.com and developer.contently.com. A prior round asserted a clientCredentials flow; nothing in Contently's published material states a flow, so that assertion has been removed.
  detail_published: false
  flows: []
  name: OAuth2
  scopes: []
  sources:
  - https://contently.com/platform/talent-api/
  type: oauth2
slug: contently-authentication
source_filename: contently-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://contently.com/platform/talent-api/\ndocs: https://contently.com/platform/talent-api/\nsummary:\n  types:\n  - oauth2\n  scoped: true\n  flows_documented: false\n  token_endpoint: null\n  authorization_endpoint: null\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    The Contently Talent API authenticates with scoped OAuth2 access tokens. Contently states this in\n    three places on the Talent API page: \"OAuth2 with scoped tokens\" (Endpoint surface), \"OAuth2 with\n    scoped tokens. Per-route rate limits. Encrypted PII.\" (Workspace governance), and\n    \"auth: oauth2 (scoped)\" (MCP tools panel).\n  flows: []\n  scopes: []\n  detail_published: false\n  detail_note: >-\n    No grant type, token endpoint, authorization endpoint, scope name, or token lifetime is published.\n    The OAuth discovery documents that would carry them\n    (/.well-known/oauth-authorization-server, /.well-known/oauth-protected-resource,\n\
  \    /.well-known/openid-configuration) return 404 on contently.com, api.contently.com and\n    developer.contently.com. A prior round asserted a clientCredentials flow; nothing in Contently's\n    published material states a flow, so that assertion has been removed.\n  sources:\n  - https://contently.com/platform/talent-api/\ncredential_acquisition:\n  self_serve: false\n  path: sales\n  note: >-\n    There is no developer signup. The Talent API page's only call to action is \"Talk to our API team\",\n    a contact form. Credentials are issued through a sales conversation.\ndeveloper_portal_finding: >-\n  CORRECTION — a prior round recorded https://developer.contently.com as the developer portal and as the\n  auth documentation source. developer.contently.com does not serve documentation: it 302s to /signin\n  and returns the Contently application login SPA (1,835 bytes, create-react-app bundle\n  main.0f164ffc.js) — byte-identical to what api.contently.com and status.contently.com serve.\
  \ It is\n  the product login, not a developer portal. The only real auth documentation is the prose on\n  https://contently.com/platform/talent-api/, which is what this file now cites.\nx-evidence:\n  checked: '2026-08-13'\n  probes:\n  - url: https://developer.contently.com/\n    status: 302\n    redirects_to: https://developer.contently.com/signin\n  - url: https://developer.contently.com/signin\n    status: 200\n    result: application login SPA, no documentation\n  - url: https://api.contently.com/.well-known/oauth-authorization-server\n    status: 404\n  - url: https://api.contently.com/.well-known/oauth-protected-resource\n    status: 404\n  - url: https://contently.com/.well-known/openid-configuration\n    status: 404\nnotes: >-\n  No OpenAPI/Swagger specification is published on any Contently host (33 discovery probes, all 404),\n  so every field here is read from published prose rather than derived from a machine-readable spec.\n  No scopes/ artifact is emitted because Contently\
  \ publishes no scope names.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contently/refs/heads/main/authentication/contently-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Content Marketing
- Talent Marketplace
- Freelance
- Content Creation
- Publishing
- Editorial Workflow
- Regulated Content
- Compliance
---
