---
anonymous_access: false
api_key_in: []
api_specs:
- filename: didlogic-com-account-balance-api-openapi.yml
  format: yaml
  label: DID Logic Account Balance API
  slug: didlogic-com-account-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-account-balance-api-openapi.yml
- filename: didlogic-com-api-access-api-openapi.yml
  format: yaml
  label: DID Logic API Access API
  slug: didlogic-com-api-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-api-access-api-openapi.yml
- filename: didlogic-com-calls-api-openapi.yml
  format: yaml
  label: DID Logic Calls API
  slug: didlogic-com-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-calls-api-openapi.yml
- filename: didlogic-com-click2call-api-openapi.yml
  format: yaml
  label: DID Logic Click2 Call API
  slug: didlogic-com-click2call-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-click2call-api-openapi.yml
- filename: didlogic-com-hlr-lookups-api-openapi.yml
  format: yaml
  label: DID Logic HLR Lookups API
  slug: didlogic-com-hlr-lookups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-hlr-lookups-api-openapi.yml
- filename: didlogic-com-identities-api-openapi.yml
  format: yaml
  label: DID Logic Identities API
  slug: didlogic-com-identities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-identities-api-openapi.yml
- filename: didlogic-com-inbound-destinations-api-openapi.yml
  format: yaml
  label: DID Logic Inbound Destinations API
  slug: didlogic-com-inbound-destinations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-inbound-destinations-api-openapi.yml
- filename: didlogic-com-kyc-documents-api-openapi.yml
  format: yaml
  label: DID Logic KYC Documents API
  slug: didlogic-com-kyc-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-kyc-documents-api-openapi.yml
- filename: didlogic-com-numbers-inventory-api-openapi.yml
  format: yaml
  label: DID Logic Numbers & Inventory API
  slug: didlogic-com-numbers-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-numbers-inventory-api-openapi.yml
- filename: didlogic-com-purchases-api-openapi.yml
  format: yaml
  label: DID Logic Purchases API
  slug: didlogic-com-purchases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-purchases-api-openapi.yml
- filename: didlogic-com-reports-api-openapi.yml
  format: yaml
  label: DID Logic Reports API
  slug: didlogic-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-reports-api-openapi.yml
- filename: didlogic-com-risk-checks-api-openapi.yml
  format: yaml
  label: DID Logic Risk Checks API
  slug: didlogic-com-risk-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-risk-checks-api-openapi.yml
- filename: didlogic-com-sip-accounts-api-openapi.yml
  format: yaml
  label: DID Logic SIP Accounts API
  slug: didlogic-com-sip-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-sip-accounts-api-openapi.yml
- filename: didlogic-com-sms-api-openapi.yml
  format: yaml
  label: DID Logic SMS API
  slug: didlogic-com-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/didlogic-com/openapi/didlogic-com-sms-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Didlogic Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: DID Logic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DID Logic
provider_slug: didlogic-com
scheme_count: 1
schemes:
- description: Authenticate API requests via API key like "Bearer YOUR_TOKEN"
  header: 'Authorization: Bearer YOUR_TOKEN'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/didlogic-com-openapi.yml
  - https://docs.didlogic.com/docs/api/get-started
  transport: HTTPS (Required)
  type: http
slug: didlogic-com-authentication
source_filename: didlogic-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource:\n- https://docs.didlogic.com/docs/api/get-started\n- openapi/didlogic-com-openapi.yml\ndocs: https://docs.didlogic.com/docs/api/get-started\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Authenticate API requests via API key like \"Bearer YOUR_TOKEN\"\n  header: 'Authorization: Bearer YOUR_TOKEN'\n  transport: HTTPS (Required)\n  sources:\n  - openapi/didlogic-com-openapi.yml\n  - https://docs.didlogic.com/docs/api/get-started\nkey_issuance:\n- 'Get started page: \"Please contact your account manager to access your API key.\"'\n- 'Release notes (July 2026): \"Generate and revoke API keys and SDK credentials on demand\" in the portal (API & Webhooks).'\nnotes:\n- All requests to both v1 and v2 endpoints must be authenticated using Bearer Token Authentication.\n- The MCP server docs describe an OAuth sign-in for MCP clients that creates an API key named \"Didlogic MCP\
  \ auth key\" in API & Webhooks (https://docs.didlogic.com/docs/guides/apps-developer-tools/mcp-server).\n  The REST spec declares no oauth2 scheme.\n- Voice SDK tokens must stay server-side; the browser widget talks to the customer's own proxy.\n"
source_yaml_url: https://artifacts.apis.io/didlogic-com/authentication/didlogic-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Telecommunications
- VoIP
- SIP Trunking
- DID Numbers
- SMS
- Voice
- MCP
---
