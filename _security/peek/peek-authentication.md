---
anonymous_access: true
api_key_in: []
api_specs:
- filename: peek-openapi-generated.yml
  format: yaml
  label: Peek API
  slug: peek-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peek/refs/heads/main/openapi/_ae-authored/peek-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Peek Authentication
name_suffix: Authentication
oauth_flows: []
overview: Peek declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Peek
provider_slug: peek
scheme_count: 3
schemes:
- api: Peek Reseller API (OCTO)
  applies_to: all operations
  example_shape: UUID v4 (Peek's doc example is a UUID)
  format: Bearer <OCTO API Key>
  header: Authorization
  in: header
  name: octoApiKey
  provisioning:
    contact: ben.smithart@peek.com
    docs: https://octodocs.peek.com/getting-started/request-access
    method: email request
    note: '"To request access, please send an email to ben.smithart@peek.com. Peek Pro''s Product team will reach out to you shortly." There is no developer signup, no console, and no published SLA on turnaround. This is a sales-gated credential.'
    self_service: false
  rotation: Peek can revoke a key server-side; no self-service rotation endpoint is documented.
  scheme: bearer
  type: http
- api: Peek Experiences MCP Server
  applies_to: all tools
  name: none
  note: 'Verified anonymously 2026-08-26: initialize and tools/list both returned 200 with no credential and no OAuth challenge. Peek''s README describes it as "a free service". No /.well-known/oauth-protected-resource is served (the transport 406s on GET).'
  type: none
- additional_header: pk-api-key (gateway key)
  api: Peek app platform GraphQL gateway (private)
  format: HS256 JWT signed with a per-install shared secret (installId as subject, app name as issuer)
  name: appJwt
  note: Documented only inside the first-party @peektravel/app-utilities package README/llms.txt. The gateway URL is not a fixed public host — it is the `apiUrl` delivered on the install webhook, so there is no public base URL to record. Not a publicly callable API; captured for completeness.
  scheme: bearer
  type: http
slug: peek-authentication
source_filename: peek-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://octodocs.peek.com/getting-started/basics + https://octodocs.peek.com/getting-started/request-access + live probe of https://octo.peek.com/integrations/octo/products\ndocs: https://octodocs.peek.com/getting-started/basics\napis:\n- api: Peek Reseller API (OCTO)\n  base_url: https://octo.peek.com/integrations/octo\n  schemes:\n  - name: octoApiKey\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: Bearer <OCTO API Key>\n    example_shape: UUID v4 (Peek's doc example is a UUID)\n    applies_to: all operations\n    rotation: Peek can revoke a key server-side; no self-service rotation endpoint is documented.\n    provisioning: &id001\n      self_service: false\n      method: email request\n      contact: ben.smithart@peek.com\n      docs: https://octodocs.peek.com/getting-started/request-access\n      note: '\"To request access, please send an email to ben.smithart@peek.com. Peek\
  \ Pro''s Product team will reach out to you shortly.\" There\n        is no developer signup, no console, and no published SLA on turnaround. This is a sales-gated credential.'\n  transport_requirements:\n  - All communication must be sent over HTTPS.\n  - 'POST, PATCH and DELETE requests must send Content-Type: application/json.'\n  failure_modes:\n  - condition: no Authorization header\n    status: 401\n    body: '{\"errorMessage\":\"Missing `Authentication` header or key could not be validated\",\"error\":\"UNAUTHORIZED\"}'\n    observed: 2026-08-26 live against https://octo.peek.com/integrations/octo/products\n  - condition: token invalid or deactivated\n    status: 403\n    error: FORBIDDEN\n    observed: documented\n  oauth2: false\n  scopes: false\n  mtls: false\n- api: Peek Experiences MCP Server\n  base_url: https://mcp.peek.com\n  schemes:\n  - name: none\n    type: none\n    applies_to: all tools\n    note: 'Verified anonymously 2026-08-26: initialize and tools/list both returned\
  \ 200 with no credential and no OAuth challenge. Peek''s README\n      describes it as \"a free service\". No /.well-known/oauth-protected-resource is served (the transport 406s on GET).'\n  oauth2: false\n- api: Peek app platform GraphQL gateway (private)\n  base_url: null\n  schemes:\n  - name: appJwt\n    type: http\n    scheme: bearer\n    format: HS256 JWT signed with a per-install shared secret (installId as subject, app name as issuer)\n    additional_header: pk-api-key (gateway key)\n    note: Documented only inside the first-party @peektravel/app-utilities package README/llms.txt. The gateway URL is not a fixed public host\n      — it is the `apiUrl` delivered on the install webhook, so there is no public base URL to record. Not a publicly callable API; captured for\n      completeness.\n  oauth2: false\ngaps:\n- No OAuth 2.0, no OIDC, no scopes, no mutual TLS anywhere on the public surface.\n- No self-service API key issuance; access to the OCTO API is granted by a human over\
  \ email.\nschemes:\n- name: octoApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: Bearer <OCTO API Key>\n  example_shape: UUID v4 (Peek's doc example is a UUID)\n  applies_to: all operations\n  rotation: Peek can revoke a key server-side; no self-service rotation endpoint is documented.\n  provisioning: *id001\n  api: Peek Reseller API (OCTO)\n- name: none\n  type: none\n  applies_to: all tools\n  note: 'Verified anonymously 2026-08-26: initialize and tools/list both returned 200 with no credential and no OAuth challenge. Peek''s README\n    describes it as \"a free service\". No /.well-known/oauth-protected-resource is served (the transport 406s on GET).'\n  api: Peek Experiences MCP Server\n- name: appJwt\n  type: http\n  scheme: bearer\n  format: HS256 JWT signed with a per-install shared secret (installId as subject, app name as issuer)\n  additional_header: pk-api-key (gateway key)\n  note: Documented only inside the first-party @peektravel/app-utilities\
  \ package README/llms.txt. The gateway URL is not a fixed public host —\n    it is the `apiUrl` delivered on the install webhook, so there is no public base URL to record. Not a publicly callable API; captured for completeness.\n  api: Peek app platform GraphQL gateway (private)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peek/refs/heads/main/authentication/peek-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Travel
- Tourism
- Booking
- Reservations
- Experience
- Tours and Activities
- Payments
- Marketplace
- MCP
- OCTO
- Software-as-a-Service
---
