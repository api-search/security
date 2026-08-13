---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Poptin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Poptin declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Poptin
provider_slug: poptin
scheme_count: 2
schemes:
- documented_reference: false
  expiry: not documented
  header_name: not documented
  id: make-zapier-api-key
  issued_from: Poptin dashboard > Settings > Profile
  name: Make/Zapier API key
  note: Poptin's help center tells a user where to COPY this key, and nothing else. No base URL, no endpoint, no header name, no example request is published alongside it.
  rotation: not documented
  scopes: none published
  transport: not documented
  type: apiKey
  used_by:
  - Make (make.com) connector
  - Zapier connector
- id: session-login
  name: Application session login
  note: Human sign-in to the Poptin application. Registration at https://app.popt.in/register. Not an API credential.
  type: http
  url: https://app.popt.in/login
slug: poptin-authentication
source_filename: poptin-authentication.yml
source_heading: Authentication Profile
source_url: https://help.poptin.com/en/article/how-to-integrate-your-poptin-to-make-etfiwq/
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://help.poptin.com/en/article/how-to-integrate-your-poptin-to-make-etfiwq/\nsources:\n- https://help.poptin.com/en/article/how-to-integrate-your-poptin-to-make-etfiwq/\n- https://help.poptin.com/en/article/how-to-integrate-your-poptin-to-zapier-9exnpm/\n- https://app.popt.in/login\nnote: >-\n  Derived-from-OpenAPI was not possible: Poptin publishes no OpenAPI, no Swagger, no\n  GraphQL SDL and no API reference of any kind (see well-known/poptin-well-known.yml and\n  the x-coverage block in apis.yml). This profile is what the provider actually documents\n  plus one anonymous live probe. Nothing about token format, header name, expiry, scopes\n  or refresh is published by Poptin, so nothing about them is asserted here.\nopenapi_security_schemes: []\nschemes:\n- id: make-zapier-api-key\n  type: apiKey\n  name: Make/Zapier API key\n  issued_from: Poptin dashboard > Settings > Profile\n  used_by:\n  - Make (make.com) connector\n\
  \  - Zapier connector\n  transport: not documented\n  header_name: not documented\n  rotation: not documented\n  expiry: not documented\n  scopes: none published\n  documented_reference: false\n  note: >-\n    Poptin's help center tells a user where to COPY this key, and nothing else. No base\n    URL, no endpoint, no header name, no example request is published alongside it.\n- id: session-login\n  type: http\n  name: Application session login\n  url: https://app.popt.in/login\n  note: >-\n    Human sign-in to the Poptin application. Registration at https://app.popt.in/register.\n    Not an API credential.\noauth2:\n  supported: false\n  note: >-\n    No OAuth authorization or token endpoint is published by Poptin, and\n    /.well-known/oauth-authorization-server returns 404 on both hosts. Third-party\n    integration-guide sites assert an OAuth flow at api.poptin.com — that hostname does\n    not resolve in DNS, so those claims are not carried into this catalog.\nscopes_artifact: not\
  \ applicable — no OAuth surface\nlive_probe:\n  url: https://app.popt.in/api/display/limitLogs/\n  method: GET\n  status: 401\n  content_type: application/json\n  fetched: '2026-08-12'\n  interpretation: >-\n    The application host does enforce authentication on its internal /api/ surface and\n    answers with JSON, which confirms a real authenticated API exists. What it does not\n    do is document it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poptin/refs/heads/main/authentication/poptin-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Marketing
- Email Marketing
- Marketing Automation
- Lead Generation
- Conversion Optimization
- Forms
- Popups
- Contact Management
- Webhooks
- Ecommerce
- SaaS
---
