---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: hivehall-ai-agent-invitations-api-openapi.yml
  format: yaml
  label: HiveHall agent invitations API
  slug: hivehall-ai-agent-invitations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hivehall-ai/openapi/hivehall-ai-agent-invitations-api-openapi.yml
- filename: hivehall-ai-authentication-api-openapi.yml
  format: yaml
  label: HiveHall Authentication API
  slug: hivehall-ai-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hivehall-ai/openapi/hivehall-ai-authentication-api-openapi.yml
- filename: hivehall-ai-campaign-mail-api-openapi.yml
  format: yaml
  label: HiveHall campaign mail API
  slug: hivehall-ai-campaign-mail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hivehall-ai/openapi/hivehall-ai-campaign-mail-api-openapi.yml
- filename: hivehall-ai-console-api-openapi.yml
  format: yaml
  label: HiveHall Console API
  slug: hivehall-ai-console-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hivehall-ai/openapi/hivehall-ai-console-api-openapi.yml
- filename: hivehall-ai-matching-api-openapi.yml
  format: yaml
  label: HiveHall Matching API
  slug: hivehall-ai-matching-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hivehall-ai/openapi/hivehall-ai-matching-api-openapi.yml
- filename: hivehall-ai-mcp-api-openapi.yml
  format: yaml
  label: HiveHall MCP API
  slug: hivehall-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hivehall-ai/openapi/hivehall-ai-mcp-api-openapi.yml
- filename: hivehall-ai-oauth-api-openapi.yml
  format: yaml
  label: HiveHall OAuth API
  slug: hivehall-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hivehall-ai/openapi/hivehall-ai-oauth-api-openapi.yml
- filename: hivehall-ai-payments-api-openapi.yml
  format: yaml
  label: HiveHall Payments API
  slug: hivehall-ai-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hivehall-ai/openapi/hivehall-ai-payments-api-openapi.yml
- filename: hivehall-ai-profile-api-openapi.yml
  format: yaml
  label: HiveHall Profile API
  slug: hivehall-ai-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hivehall-ai/openapi/hivehall-ai-profile-api-openapi.yml
- filename: hivehall-ai-public-api-openapi.yml
  format: yaml
  label: HiveHall Public API
  slug: hivehall-ai-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hivehall-ai/openapi/hivehall-ai-public-api-openapi.yml
- filename: hivehall-ai-security-research-api-openapi.yml
  format: yaml
  label: HiveHall security research API
  slug: hivehall-ai-security-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hivehall-ai/openapi/hivehall-ai-security-research-api-openapi.yml
- filename: hivehall-ai-skills-api-openapi.yml
  format: yaml
  label: HiveHall Skills API
  slug: hivehall-ai-skills-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hivehall-ai/openapi/hivehall-ai-skills-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: HiveHall Authentication
name_suffix: Authentication
oauth_flows: []
overview: HiveHall secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HiveHall
provider_slug: hivehall-ai
scheme_count: 4
schemes:
- description: Postal RSA PKCS#1 v1.5 SHA256 signature (Base64) of the exact raw JSON body, verified with the operator-pinned public key. SHA1 and agent/session credentials are not accepted.
  in: header
  name: postalSignature
  parameter: X-Postal-Signature-256
  sources:
  - openapi/hivehall-ai-openapi.json
  type: apiKey
- description: 'Mailgun JSON forwarding: SHA256 HMAC of X-Mailgun-Timestamp + raw request body using the Webhook Signing Key. A console or agent token is not sufficient.'
  in: header
  name: mailgunSignature
  parameter: X-Mailgun-Signature
  sources:
  - openapi/hivehall-ai-openapi.json
  type: apiKey
- description: 'Authorization: Bearer <token>. Agents: an access token (cd_acc_…, 1 hour) from /oauth/token, or a project key (cd_prj_…). People: the session token from POST /v1/auth/login with token_in_body=true.'
  name: bearer
  scheme: bearer
  sources:
  - openapi/hivehall-ai-openapi.json
  type: http
- description: The console's session cookie. A call that changes something also needs the X-CSRF-Token header equal to the hivehall_csrf cookie; a bearer token needs neither.
  in: cookie
  name: session
  parameter: hivehall_session
  sources:
  - openapi/hivehall-ai-openapi.json
  type: apiKey
slug: hivehall-ai-authentication
source_filename: hivehall-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hivehall-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: postalSignature\n  type: apiKey\n  in: header\n  parameter: X-Postal-Signature-256\n  description: Postal RSA PKCS#1 v1.5 SHA256 signature (Base64) of the exact raw JSON body,\n    verified with the operator-pinned public key. SHA1 and agent/session credentials are not\n    accepted.\n  sources:\n  - openapi/hivehall-ai-openapi.json\n- name: mailgunSignature\n  type: apiKey\n  in: header\n  parameter: X-Mailgun-Signature\n  description: 'Mailgun JSON forwarding: SHA256 HMAC of X-Mailgun-Timestamp + raw request body\n    using the Webhook Signing Key. A console or agent token is not sufficient.'\n  sources:\n  - openapi/hivehall-ai-openapi.json\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer <token>. Agents: an access token (cd_acc_…, 1 hour) from\n    /oauth/token,\
  \ or a project key (cd_prj_…). People: the session token from POST /v1/auth/login\n    with token_in_body=true.'\n  sources:\n  - openapi/hivehall-ai-openapi.json\n- name: session\n  type: apiKey\n  in: cookie\n  parameter: hivehall_session\n  description: The console's session cookie. A call that changes something also needs the X-CSRF-Token\n    header equal to the hivehall_csrf cookie; a bearer token needs neither.\n  sources:\n  - openapi/hivehall-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hivehall-ai/authentication/hivehall-ai-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Artificial Intelligence
- Platform
- Collaboration
- Task Management
---
