---
anonymous_access: false
api_key_in: []
api_specs:
- filename: billionverify-com-account-api-openapi.yml
  format: yaml
  label: BillionVerify Account API
  slug: billionverify-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billionverify-com/openapi/billionverify-com-account-api-openapi.yml
- filename: billionverify-com-file-processing-api-openapi.yml
  format: yaml
  label: BillionVerify File Processing API
  slug: billionverify-com-file-processing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billionverify-com/openapi/billionverify-com-file-processing-api-openapi.yml
- filename: billionverify-com-health-api-openapi.yml
  format: yaml
  label: BillionVerify Health API
  slug: billionverify-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billionverify-com/openapi/billionverify-com-health-api-openapi.yml
- filename: billionverify-com-verification-api-openapi.yml
  format: yaml
  label: BillionVerify Verification API
  slug: billionverify-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billionverify-com/openapi/billionverify-com-verification-api-openapi.yml
- filename: billionverify-com-webhooks-api-openapi.yml
  format: yaml
  label: BillionVerify Webhooks API
  slug: billionverify-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billionverify-com/openapi/billionverify-com-webhooks-api-openapi.yml
auth_types: []
description: Authentication methods for BillionVerify REST API and MCP server
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: BillionVerify Authentication
name_suffix: Authentication
oauth_flows: []
overview: BillionVerify declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: BillionVerify
provider_slug: billionverify-com
scheme_count: 4
schemes:
- evidence: 'Send your API key in the BV-API-KEY header:'
  header: BV-API-KEY
  location: header
  name: BV-API-KEY
  type: apiKey
- evidence: 'The following header names are all accepted, in priority order: BV-API-KEY (recommended) BILLIONVERIFY-API-KEY'
  header: BILLIONVERIFY-API-KEY
  location: header
  name: BILLIONVERIFY-API-KEY
  type: apiKey
- evidence: 'Authorization: Bearer <api_key>'
  header: Authorization
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'BillionVerify MCP uses a standard remote OAuth flow:'
  flows:
  - client_credentials
  header: Authorization
  location: header
  name: OAuth2
  scopes:
  - billionverify.read
  - billionverify.verify
  - billionverify.webhooks
  type: oauth2
slug: billionverify-com-authentication
source_filename: billionverify-com-authentication.yml
source_heading: Authentication Profile
source_url: https://billionverify.com/docs/quickstart
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://billionverify.com/docs/quickstart\nsources:\n- https://billionverify.com/docs/quickstart\n- https://billionverify.com/docs/api-reference\n- https://billionverify.com/docs/ai-guides/mcp\n- https://billionverify.com/docs/sdks/java\ndescription: Authentication methods for BillionVerify REST API and MCP server\nschemes:\n- type: apiKey\n  name: BV-API-KEY\n  evidence: 'Send your API key in the BV-API-KEY header:'\n  location: header\n  header: BV-API-KEY\n- type: apiKey\n  name: BILLIONVERIFY-API-KEY\n  evidence: 'The following header names are all accepted, in priority order: BV-API-KEY (recommended) BILLIONVERIFY-API-KEY'\n  location: header\n  header: BILLIONVERIFY-API-KEY\n- type: http-bearer\n  name: Authorization\n  evidence: 'Authorization: Bearer <api_key>'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: OAuth2\n  evidence: 'BillionVerify MCP uses\
  \ a standard remote OAuth flow:'\n  location: header\n  header: Authorization\n  flows:\n  - client_credentials\n  scopes:\n  - billionverify.read\n  - billionverify.verify\n  - billionverify.webhooks\ndocs: https://billionverify.com/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/billionverify-com/authentication/billionverify-com-authentication.yml
summary_line: 4 schemes
tags:
- Email Verification
- Software-as-a-Service
- Data Quality
- B2B
---
