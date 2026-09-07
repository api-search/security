---
anonymous_access: false
api_key_in:
- header
- query
- cookie
api_specs:
- filename: vulncheck-api-openapi.json
  format: json
  label: VulnCheck API
  slug: vulncheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vulncheck/refs/heads/main/openapi/vulncheck-api-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Vulncheck Authentication
name_suffix: Authentication
oauth_flows: []
overview: VulnCheck secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VulnCheck
provider_slug: vulncheck
scheme_count: 3
schemes:
- declared_in_spec: true
  format: 'Authorization: Bearer <token>'
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/vulncheck-api-openapi.json
  - https://docs.vulncheck.com/getting-started/api-tokens
  type: apiKey
- declared_in_spec: false
  documented: true
  format: ?token=<token>
  in: query
  name: token (query parameter)
  note: Documented as a convenience for testing tokens and browsing endpoints in a browser. Real and supported, but a credential in a URL is recorded in proxy logs, browser history and Referer headers. Recorded because VulnCheck publishes it, not because it is advisable.
  parameter: token
  sources:
  - https://docs.vulncheck.com/getting-started/api-tokens
  type: apiKey
- declared_in_spec: false
  documented: true
  format: 'Cookie: token=<token>'
  in: cookie
  name: token (cookie)
  note: This is how VulnCheck's own web portal authenticates against the same API.
  parameter: token
  sources:
  - https://docs.vulncheck.com/getting-started/api-tokens
  type: apiKey
slug: vulncheck-authentication
source_filename: vulncheck-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://docs.vulncheck.com/getting-started/api-tokens\ndocs: https://docs.vulncheck.com/getting-started/api-tokens\nderived_from: openapi/vulncheck-api-openapi.json\napi: VulnCheck API v3\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  - cookie\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: none\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Authorization: Bearer <token>'\n  declared_in_spec: true\n  sources:\n  - openapi/vulncheck-api-openapi.json\n  - https://docs.vulncheck.com/getting-started/api-tokens\n- name: token (query parameter)\n  type: apiKey\n  in: query\n  parameter: token\n  format: '?token=<token>'\n  declared_in_spec: false\n  documented: true\n  sources:\n  - https://docs.vulncheck.com/getting-started/api-tokens\n  note: >-\n    Documented as a convenience for testing tokens and browsing endpoints in a browser.\
  \ Real\n    and supported, but a credential in a URL is recorded in proxy logs, browser history and\n    Referer headers. Recorded because VulnCheck publishes it, not because it is advisable.\n- name: token (cookie)\n  type: apiKey\n  in: cookie\n  parameter: token\n  format: 'Cookie: token=<token>'\n  declared_in_spec: false\n  documented: true\n  sources:\n  - https://docs.vulncheck.com/getting-started/api-tokens\n  note: This is how VulnCheck's own web portal authenticates against the same API.\ntoken:\n  kind: long-lived API token\n  shared_with: The same token authenticates both the API and the web portal.\n  issue: https://console.vulncheck.com/settings/tokens\n  issue_flow: Tokens & SSH Keys page -> Create Token -> label + icon. The value is shown ONCE.\n  rotation: Self-service create and remove; no automated rotation endpoint.\n  expiry: A token unused for 30 days expires and must be recreated.\n  revocation: Remove the token from the Tokens & SSH Keys page, or via `vulncheck\
  \ token remove`.\n  env_var: VC_TOKEN\n  cli: vulncheck auth login (browser or paste-token)\nfailure:\n  status: 401\n  body: '{\"error\":true,\"errors\":[\"unauthorized\"]}'\n  www_authenticate: false\n  method: probed\n  probe:\n    url: https://api.vulncheck.com/v3/index/a10\n    status: 401\n    note: >-\n      No WWW-Authenticate challenge is returned, so a client cannot discover the required\n      scheme from the response. The 401 body is also typed as a bare `string` in the spec.\nanonymous_surface:\n- url: https://api.vulncheck.com/v3/openapi\n  status: 200\n  note: The OpenAPI document itself is the only operation reachable without a token.\ngaps:\n- id: no-global-security-requirement\n  detail: >-\n    The OpenAPI declares no top-level `security` and applies the Bearer scheme to no operation,\n    so a generated client reads all 521 operations as anonymous when 520 of them return 401.\n    Captured as a correction in overlays/vulncheck-api-overlay.yaml.\n- id: undeclared-transports\n\
  \  detail: The query-parameter and cookie transports are documented but absent from the spec.\n- id: no-scopes\n  detail: >-\n    There is no scope or permission model. Access is all-or-nothing per token, differentiated\n    only by the account's entitlements (GET /entitlements returns a map of roles to\n    entitlements). An agent cannot be issued a narrowed credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vulncheck/refs/heads/main/authentication/vulncheck-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Security
- Vulnerability Intelligence
- Exploit Intelligence
- Threat Intelligence
- Cybersecurity
- CVE
- Vulnerability Management
- Data
---
