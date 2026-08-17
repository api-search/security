---
api_key_in:
- header
- query
api_specs:
- filename: mailmodo-campaigns-api-openapi.yml
  format: yaml
  label: Mailmodo Campaigns API
  slug: mailmodo-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-campaigns-api-openapi.yml
- filename: mailmodo-contact-lists-api-openapi.yml
  format: yaml
  label: Mailmodo Contact Lists API
  slug: mailmodo-contact-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-contact-lists-api-openapi.yml
- filename: mailmodo-contacts-api-openapi.yml
  format: yaml
  label: Mailmodo Contacts API
  slug: mailmodo-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-contacts-api-openapi.yml
- filename: mailmodo-events-api-openapi.yml
  format: yaml
  label: Mailmodo Events API
  slug: mailmodo-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-events-api-openapi.yml
- filename: mailmodo-templates-api-openapi.yml
  format: yaml
  label: Mailmodo Templates API
  slug: mailmodo-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-templates-api-openapi.yml
- filename: mailmodo-user-journeys-api-openapi.yml
  format: yaml
  label: Mailmodo User Journeys API
  slug: mailmodo-user-journeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-user-journeys-api-openapi.yml
- filename: mailmodo-dynamic-form-api-openapi.yml
  format: yaml
  label: Mailmodo Dynamic Form API
  slug: mailmodo-dynamic-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-dynamic-form-api-openapi.yml
- filename: mailmodo-repeatable-block-api-openapi.yml
  format: yaml
  label: Mailmodo Repeatable Block API
  slug: mailmodo-repeatable-block-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/openapi/mailmodo-repeatable-block-api-openapi.yml
auth_types:
- apiKey
description: 'One credential class, one mechanism: a workspace API key sent in the `mmApiKey` header. There is no OAuth, no OpenID Connect, no mutual TLS, no scopes, no permissions model and no test/live key split. A Mailmodo API key is a single account-wide bearer of full API authority — anything holding it can read every contact and send mail as the workspace.'
kind: authentication
layout: security
method: searched
name: Mailmodo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailmodo secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mailmodo
provider_slug: mailmodo
scheme_count: 2
schemes:
- description: API key issued from the Mailmodo dashboard at Settings > API Keys. Sent as the `mmApiKey` request header on every call. This is the canonical form, used by seven of the eight published specs and by Mailmodo's own MCP server and SDKs.
  in: header
  name: mmApiKey
  parameter: mmApiKey
  sources:
  - openapi/_original/mailmodo-sending-emails-openapi.json
  - openapi/_original/mailmodo-contact-management-openapi.json
  - openapi/_original/mailmodo-custom-events-openapi.json
  - openapi/_original/mailmodo-templates-openapi.json
  - openapi/_original/mailmodo-user-journeys-openapi.json
  - openapi/_original/mailmodo-dynamic-form-openapi.json
  - openapi/_original/mailmodo-repeatable-block-openapi.json
  type: apiKey
- description: The Campaign Data spec declares the SAME credential as a query parameter rather than a header. Treat this as a spec defect and send the header — putting a long-lived credential in a URL leaks it into logs, proxies and referrers.
  in: query
  name: mmApiKey (query variant)
  parameter: mmApiKey
  sources:
  - openapi/_original/mailmodo-campaign-data-openapi.yaml
  status: inconsistent
  type: apiKey
slug: mailmodo-authentication
source_filename: mailmodo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://www.mailmodo.com/developers/8e957152b6128-getting-started-with-mailmodo-api (provider's own\n  getting-started guide) and the eight provider-published OpenAPI documents in openapi/_original/,\n  harvested 2026-08-13. Key format confirmed from https://www.npmjs.com/package/@mailmodo/cli.\ndocs: https://www.mailmodo.com/developers/8e957152b6128-getting-started-with-mailmodo-api\nconsole: https://manage.mailmodo.com/app/settings/apikey\nname: Mailmodo Authentication\ndescription: >-\n  One credential class, one mechanism: a workspace API key sent in the `mmApiKey` header. There is no\n  OAuth, no OpenID Connect, no mutual TLS, no scopes, no permissions model and no test/live key\n  split. A Mailmodo API key is a single account-wide bearer of full API authority — anything holding\n  it can read every contact and send mail as the workspace.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n    - query\n\
  \  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: false\nschemes:\n  - name: mmApiKey\n    type: apiKey\n    in: header\n    parameter: mmApiKey\n    description: >-\n      API key issued from the Mailmodo dashboard at Settings > API Keys. Sent as the `mmApiKey`\n      request header on every call. This is the canonical form, used by seven of the eight published\n      specs and by Mailmodo's own MCP server and SDKs.\n    sources:\n      - openapi/_original/mailmodo-sending-emails-openapi.json\n      - openapi/_original/mailmodo-contact-management-openapi.json\n      - openapi/_original/mailmodo-custom-events-openapi.json\n      - openapi/_original/mailmodo-templates-openapi.json\n      - openapi/_original/mailmodo-user-journeys-openapi.json\n      - openapi/_original/mailmodo-dynamic-form-openapi.json\n      - openapi/_original/mailmodo-repeatable-block-openapi.json\n  - name: mmApiKey (query variant)\n    type: apiKey\n    in: query\n    parameter: mmApiKey\n\
  \    description: >-\n      The Campaign Data spec declares the SAME credential as a query parameter rather than a header.\n      Treat this as a spec defect and send the header — putting a long-lived credential in a URL\n      leaks it into logs, proxies and referrers.\n    sources:\n      - openapi/_original/mailmodo-campaign-data-openapi.yaml\n    status: inconsistent\nkey_management:\n  obtain: Settings > API Keys > \"Show API Key\" in https://manage.mailmodo.com/app/settings/apikey\n  multiple_keys: true\n  create: '\"Add new API Key\" button in the dashboard'\n  format: 'XXXXXXX-XXXXXXX-XXXXXXX-XXXXXXX — four hyphen-separated groups of 7 uppercase alphanumerics'\n  format_source: https://www.npmjs.com/package/@mailmodo/cli\n  environment_variable: MAILMODO_API_KEY\n  expiry: none-published\n  rotation_policy: none-published\n  revocation: not-documented\n  test_keys: false\n  scoping: >-\n    None. There is no read-only key, no per-list key and no per-operation restriction. The dashboard\n\
  \    has role-based access control (admin / read-write / read-only) for HUMANS, per\n    https://www.mailmodo.com/security/, but that model does not extend to API keys.\ntransport:\n  tls_required: true\n  minimum_tls: 'TLS 1.2+ (stated on https://www.mailmodo.com/security/)'\nagent_surfaces:\n  - surface: MCP (remote)\n    endpoint: https://mcp.app.mailmodo.com/mcp\n    credential: same mmApiKey, passed as a header via mcp-remote\n    probed: '2026-08-13 — HTTP 400 {\"code\":-32000,\"message\":\"Bad Request: No valid mmApiKey provided\"}'\n  - surface: MCP (local stdio)\n    credential: MAILMODO_API_KEY environment variable\n  - surface: '@mailmodo/cli'\n    credential: MAILMODO_API_KEY env var or ~/.mailmodo/config\n    note: Targets api.mailmodo.dev, not api.mailmodo.com.\ngaps:\n  - >-\n    No OAuth means no delegated authorization: a third-party integration cannot act for a Mailmodo\n    customer without holding that customer's full-authority key.\n  - No published expiry, rotation\
  \ or revocation procedure.\n  - No 401/403 response is declared on ANY operation in ANY published spec.\n  - No /.well-known/oauth-authorization-server or openid-configuration on any host (all 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailmodo/refs/heads/main/authentication/mailmodo-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Email
- Interactive Email
- AMP for Email
- Marketing Automation
- Transactional Email
- Campaigns
- Journeys
- Customer Engagement
---
