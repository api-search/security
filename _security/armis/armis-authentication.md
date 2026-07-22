---
api_key_in: []
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Armis Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Armis secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Armis
provider_slug: armis
scheme_count: 2
schemes:
- env:
  - ARMIS_AUDIENCE
  - ARMIS_CLIENT_ID
  - ARMIS_CLIENT_SECRET
  - ARMIS_VENDOR_ID
  flow: clientCredentials
  name: clientCredentials
  parameters:
    audience: Tenant URL including trailing slash (e.g. https://acme.armis.com/)
    client_id: Client ID (email of the account that generated the client secret)
    client_secret: Confidential credential generated within the Armis tenant
    scopes: Specific permissions the access token needs for the desired API endpoints
    vendor_id: Identifier for the developer account / integration, obtained on the developer portal
  sources:
  - https://github.com/ArmisSecurity/armis-sdk-python
  - https://github.com/ArmisSecurity/armis-knowledge-mcp
  token_endpoint: /api/v1/auth/token
  token_lifetime: short-lived JWT (~55 min cache observed in official clients)
  type: oauth2
- env:
  - ARMIS_API_TOKEN
  - ARMIS_TENANT_ID
  in: header
  name: apiToken
  note: Legacy Basic/token auth path retained by armis-cli (--token/--tenant-id).
  parameters:
    tenant_id: Tenant identifier
    token: API token
  sources:
  - https://github.com/ArmisSecurity/armis-cli
  status: legacy
  type: apiKey
slug: armis-authentication
source_filename: armis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/ArmisSecurity/armis-sdk-python\ndocs: https://developers.armis.com/\nsummary:\n  types: [oauth2, apiKey]\n  oauth2_flows: [clientCredentials]\n  primary: OAuth2 client-credentials -> short-lived JWT bearer, tenant-scoped audience\nschemes:\n  - name: clientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_endpoint: /api/v1/auth/token\n    parameters:\n      audience: Tenant URL including trailing slash (e.g. https://acme.armis.com/)\n      client_id: Client ID (email of the account that generated the client secret)\n      client_secret: Confidential credential generated within the Armis tenant\n      vendor_id: Identifier for the developer account / integration, obtained on the developer portal\n      scopes: Specific permissions the access token needs for the desired API endpoints\n    env: [ARMIS_AUDIENCE, ARMIS_CLIENT_ID, ARMIS_CLIENT_SECRET, ARMIS_VENDOR_ID]\n    token_lifetime: short-lived\
  \ JWT (~55 min cache observed in official clients)\n    sources: [https://github.com/ArmisSecurity/armis-sdk-python, https://github.com/ArmisSecurity/armis-knowledge-mcp]\n  - name: apiToken\n    type: apiKey\n    in: header\n    status: legacy\n    parameters:\n      token: API token\n      tenant_id: Tenant identifier\n    env: [ARMIS_API_TOKEN, ARMIS_TENANT_ID]\n    note: Legacy Basic/token auth path retained by armis-cli (--token/--tenant-id).\n    sources: [https://github.com/ArmisSecurity/armis-cli]\nnotes:\n  - Access tokens are OAuth scope-gated (permissions per endpoint); the scope enumeration is issued per developer registration and is not published as a flat catalog, so no scopes/ artifact is derived.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armis/refs/heads/main/authentication/armis-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Defense Government
- Security
- Cybersecurity
- Asset Intelligence
- Exposure Management
- IoT
- OT Security
- Vulnerability Management
- Developer Tools
---
