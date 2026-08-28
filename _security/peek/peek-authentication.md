---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Peek Authentication
name_suffix: Authentication
oauth_flows: []
overview: Peek declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Peek
provider_slug: peek
scheme_count: 0
schemes: []
slug: peek-authentication
source_filename: peek-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://octodocs.peek.com/getting-started/basics + https://octodocs.peek.com/getting-started/request-access + live probe of https://octo.peek.com/integrations/octo/products\ndocs: https://octodocs.peek.com/getting-started/basics\napis:\n- api: Peek Reseller API (OCTO)\n  base_url: https://octo.peek.com/integrations/octo\n  schemes:\n  - name: octoApiKey\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Bearer <OCTO API Key>'\n    example_shape: UUID v4 (Peek's doc example is a UUID)\n    applies_to: all operations\n    rotation: Peek can revoke a key server-side; no self-service rotation endpoint is documented.\n    provisioning:\n      self_service: false\n      method: email request\n      contact: ben.smithart@peek.com\n      docs: https://octodocs.peek.com/getting-started/request-access\n      note: >-\n        \"To request access, please send an email to ben.smithart@peek.com.\
  \ Peek Pro's Product team will\n        reach out to you shortly.\" There is no developer signup, no console, and no published SLA on\n        turnaround. This is a sales-gated credential.\n  transport_requirements:\n  - All communication must be sent over HTTPS.\n  - 'POST, PATCH and DELETE requests must send Content-Type: application/json.'\n  failure_modes:\n  - condition: no Authorization header\n    status: 401\n    body: '{\"errorMessage\":\"Missing `Authentication` header or key could not be validated\",\"error\":\"UNAUTHORIZED\"}'\n    observed: '2026-08-26 live against https://octo.peek.com/integrations/octo/products'\n  - condition: token invalid or deactivated\n    status: 403\n    error: FORBIDDEN\n    observed: documented\n  oauth2: false\n  scopes: false\n  mtls: false\n- api: Peek Experiences MCP Server\n  base_url: https://mcp.peek.com\n  schemes:\n  - name: none\n    type: none\n    applies_to: all tools\n    note: >-\n      Verified anonymously 2026-08-26: initialize\
  \ and tools/list both returned 200 with no credential and\n      no OAuth challenge. Peek's README describes it as \"a free service\". No\n      /.well-known/oauth-protected-resource is served (the transport 406s on GET).\n  oauth2: false\n- api: Peek app platform GraphQL gateway (private)\n  base_url: null\n  schemes:\n  - name: appJwt\n    type: http\n    scheme: bearer\n    format: HS256 JWT signed with a per-install shared secret (installId as subject, app name as issuer)\n    additional_header: 'pk-api-key (gateway key)'\n    note: >-\n      Documented only inside the first-party @peektravel/app-utilities package README/llms.txt. The\n      gateway URL is not a fixed public host — it is the `apiUrl` delivered on the install webhook, so\n      there is no public base URL to record. Not a publicly callable API; captured for completeness.\n  oauth2: false\ngaps:\n- No OAuth 2.0, no OIDC, no scopes, no mutual TLS anywhere on the public surface.\n- No self-service API key issuance; access\
  \ to the OCTO API is granted by a human over email.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peek/refs/heads/main/authentication/peek-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Travel
- Tourism
- Booking
- Reservations
- Experiences
- Tours and Activities
- Payments
- Marketplace
- MCP
- OCTO
- SaaS
---
