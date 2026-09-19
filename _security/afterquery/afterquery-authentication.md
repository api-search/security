---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Afterquery Authentication
name_suffix: Authentication
oauth_flows: []
overview: AfterQuery declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AfterQuery
provider_slug: afterquery
scheme_count: 1
schemes:
- evidence:
    checked: '2026-09-12'
    declared: 'https://docs.afterquery.com/.well-known/mcp.json -> servers[0].authentication: none'
    observed: anonymous tools/list returned HTTP 200 with three tools
  id: none
  required: false
  surface: https://docs.afterquery.com/mcp
  type: none
slug: afterquery-authentication
source_filename: afterquery-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: >-\n  https://docs.afterquery.com/.well-known/mcp.json (HTTP 200, declares authentication \"none\") and an\n  anonymous POST tools/list to https://docs.afterquery.com/mcp (HTTP 200, full tool set returned\n  with no credential), both on 2026-09-12.\nnote: >-\n  There is no API key, OAuth client or token of any kind to obtain from AfterQuery, because there is\n  no public product API. The only callable surface is the documentation MCP server, and it is\n  anonymous by declaration and by observation. This artifact records that measured fact so the\n  record is not read as \"auth unknown\".\nschemes:\n- id: none\n  type: none\n  surface: https://docs.afterquery.com/mcp\n  required: false\n  evidence:\n    declared: 'https://docs.afterquery.com/.well-known/mcp.json -> servers[0].authentication: none'\n    observed: anonymous tools/list returned HTTP 200 with three tools\n    checked: '2026-09-12'\noauth:\n  supported: false\n  authorization_server_metadata:\
  \ 'https://docs.afterquery.com/.well-known/oauth-authorization-server - HTTP 404'\n  protected_resource_metadata: 'https://docs.afterquery.com/.well-known/oauth-protected-resource - HTTP 404'\n  openid_configuration: 'https://www.afterquery.com/.well-known/openid-configuration - HTTP 404'\nscopes:\n  applicable: false\n  note: No OAuth surface exists, so scopes/ is intentionally absent rather than empty.\nhuman_login:\n  surface: https://experts.afterquery.com/\n  note: >-\n    The AfterQuery Experts contributor platform has a human sign-in and an onboarding flow with\n    identity verification via Persona and payouts via Stripe (documented at\n    https://docs.afterquery.com/articles/onboarding/complete-your-onboarding). It is a web\n    application login, not a programmatic authentication surface, and it was not probed further -\n    the host answers 429 with a Vercel Security Checkpoint to non-browser clients.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afterquery/refs/heads/main/authentication/afterquery-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- Training Data
- Data
- Evaluation
- Reinforcement Learning
- Benchmarks
- Research
- Agents
- MCP
---
