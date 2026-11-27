---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: ctlogs-io-certs-api-openapi.yml
  format: yaml
  label: CTlogs.io Certs API
  slug: ctlogs-io-certs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctlogs-io/openapi/ctlogs-io-certs-api-openapi.yml
- filename: ctlogs-io-me-api-openapi.yml
  format: yaml
  label: CTlogs.io Me API
  slug: ctlogs-io-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctlogs-io/openapi/ctlogs-io-me-api-openapi.yml
- filename: ctlogs-io-search-api-openapi.yml
  format: yaml
  label: CTlogs.io Search API
  slug: ctlogs-io-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctlogs-io/openapi/ctlogs-io-search-api-openapi.yml
- filename: ctlogs-io-stats-api-openapi.yml
  format: yaml
  label: CTlogs.io Stats API
  slug: ctlogs-io-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctlogs-io/openapi/ctlogs-io-stats-api-openapi.yml
- filename: ctlogs-io-subdomains-api-openapi.yml
  format: yaml
  label: CTlogs.io Subdomains API
  slug: ctlogs-io-subdomains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ctlogs-io/openapi/ctlogs-io-subdomains-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CTlogs.io Authentication
name_suffix: Authentication
oauth_flows: []
overview: CTlogs.io secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CTlogs.io
provider_slug: ctlogs-io
scheme_count: 2
schemes:
- description: 'The API requires a subscription ( from $29.99 per month ). There is no free tier of the API and no trial. Your key is issued in the member area. Send it in a header, over HTTPS: X-API-Key: ct_live_… HTTPS only. A request that arrives over http:// is refused rather than redirected.'
  in: header
  key_prefix: ct_live_
  name: ApiKeyHeader
  notes:
  - One key per account. Rotate or revoke it in the member area at any time; the old key stops working within about a minute.
  - The OpenAPI also states a ?key= query parameter is accepted, but the docs say to keep the key out of the URL.
  - More than 30 rejected keys in a minute from one address stops that address for ten minutes.
  parameter: X-API-Key
  sources:
  - openapi/ctlogs-io-openapi.yml
  - https://ctlogs.io/docs
  type: apiKey
- applies_to: https://mcp.ctlogs.io/mcp
  description: The client opens CTlogs, you sign in and approve the connection once. The MCP connector is "authorised by signing in — no key to paste".
  name: MCP sign-in
  sources:
  - https://ctlogs.io/mcp
  - https://ctlogs.io/docs
  type: oauth-style-signin
slug: ctlogs-io-authentication
source_filename: ctlogs-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://ctlogs.io/docs\ndocs: https://ctlogs.io/docs#authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  key_prefix: ct_live_\n  description: \"The API requires a subscription ( from $29.99 per month ). There is no free tier of the API and no trial. Your key is issued in the member area. Send it in a header, over HTTPS: X-API-Key: ct_live_… HTTPS only. A request that arrives over http:// is refused rather than redirected.\"\n  notes:\n  - One key per account. Rotate or revoke it in the member area at any time; the old key stops working within about a minute.\n  - The OpenAPI also states a ?key= query parameter is accepted, but the docs say to keep the key out of the URL.\n  - More than 30 rejected keys in a minute from one address stops that address for ten minutes.\n  sources:\n  - openapi/ctlogs-io-openapi.yml\n\
  \  - https://ctlogs.io/docs\n- name: MCP sign-in\n  type: oauth-style-signin\n  applies_to: https://mcp.ctlogs.io/mcp\n  description: 'The client opens CTlogs, you sign in and approve the connection once. The MCP connector is \"authorised by signing in — no key to paste\".' \n  sources:\n  - https://ctlogs.io/mcp\n  - https://ctlogs.io/docs\n"
source_yaml_url: https://artifacts.apis.io/ctlogs-io/authentication/ctlogs-io-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Certificate Transparency
- TLS Certificates
- SSL
- Security
- PKI
- Domains
- MCP
---
