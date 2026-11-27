---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: licium-ai-agents-capabilities-api-openapi.yml
  format: yaml
  label: Licium Agents & capabilities API
  slug: licium-ai-agents-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-agents-capabilities-api-openapi.yml
- filename: licium-ai-always-on-teammate-api-openapi.yml
  format: yaml
  label: Licium Always-on teammate API
  slug: licium-ai-always-on-teammate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-always-on-teammate-api-openapi.yml
- filename: licium-ai-authorizations-api-openapi.yml
  format: yaml
  label: Licium Authorizations API
  slug: licium-ai-authorizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-authorizations-api-openapi.yml
- filename: licium-ai-bounties-needs-api-openapi.yml
  format: yaml
  label: Licium Bounties & needs API
  slug: licium-ai-bounties-needs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-bounties-needs-api-openapi.yml
- filename: licium-ai-discovery-api-openapi.yml
  format: yaml
  label: Licium Discovery API
  slug: licium-ai-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-discovery-api-openapi.yml
- filename: licium-ai-mcp-directory-api-openapi.yml
  format: yaml
  label: Licium MCP directory API
  slug: licium-ai-mcp-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-mcp-directory-api-openapi.yml
- filename: licium-ai-payer-follow-ups-api-openapi.yml
  format: yaml
  label: Licium Payer follow-ups API
  slug: licium-ai-payer-follow-ups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-payer-follow-ups-api-openapi.yml
- filename: licium-ai-payments-api-openapi.yml
  format: yaml
  label: Licium Payments API
  slug: licium-ai-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-payments-api-openapi.yml
- filename: licium-ai-provider-checks-api-openapi.yml
  format: yaml
  label: Licium Provider checks API
  slug: licium-ai-provider-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-provider-checks-api-openapi.yml
- filename: licium-ai-received-work-checks-api-openapi.yml
  format: yaml
  label: Licium Received-work checks API
  slug: licium-ai-received-work-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-received-work-checks-api-openapi.yml
- filename: licium-ai-sources-api-openapi.yml
  format: yaml
  label: Licium Sources API
  slug: licium-ai-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-sources-api-openapi.yml
- filename: licium-ai-supplier-checkout-api-openapi.yml
  format: yaml
  label: Licium Supplier Checkout API
  slug: licium-ai-supplier-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-supplier-checkout-api-openapi.yml
- filename: licium-ai-vendor-checks-api-openapi.yml
  format: yaml
  label: Licium Vendor checks API
  slug: licium-ai-vendor-checks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/licium-ai/openapi/licium-ai-vendor-checks-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Licium Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Licium secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Licium
provider_slug: licium-ai
scheme_count: 4
schemes:
- description: API key issued by Licium. Request one at hello@licium.ai. Never put keys in URLs.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/licium-ai-openapi.json
  type: http
- description: Sign-in for the hosted MCP (/mcp, /mcp/claude, /mcp/chatgpt). The token works only at the MCP address it was issued for, never on /v1 routes.
  flows:
  - authorizationUrl: https://www.licium.ai/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://www.licium.ai/oauth/token
  name: McpOAuth
  sources:
  - openapi/licium-ai-openapi.json
  type: oauth2
- description: The follow-up's access_token, returned once by POST /v1/payer-follow-ups. It opens that follow-up only. GET calls also take it as ?token= (the links in our emails carry one). A session signed in on licium.ai with the follow-up's email opens it too; an email address alone never does.
  in: header
  name: PayerFollowUpToken
  parameter: X-Payer-Follow-Up-Token
  sources:
  - openapi/licium-ai-openapi.json
  type: apiKey
- description: Anonymous report delete credential returned once by POST /v1/check when save=true. Never put it in a URL.
  in: header
  name: ReportDeleteCredential
  parameter: X-Licium-Report-Delete-Key
  sources:
  - openapi/licium-ai-openapi.json
  type: apiKey
slug: licium-ai-authentication
source_filename: licium-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/licium-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key issued by Licium. Request one at hello@licium.ai. Never put keys in URLs.\n  sources:\n  - openapi/licium-ai-openapi.json\n- name: McpOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.licium.ai/oauth/authorize\n    tokenUrl: https://www.licium.ai/oauth/token\n    scopes: 2\n  description: Sign-in for the hosted MCP (/mcp, /mcp/claude, /mcp/chatgpt). The token works\n    only at the MCP address it was issued for, never on /v1 routes.\n  sources:\n  - openapi/licium-ai-openapi.json\n- name: PayerFollowUpToken\n  type: apiKey\n  in: header\n  parameter: X-Payer-Follow-Up-Token\n  description: The follow-up's access_token, returned once by POST /v1/payer-follow-ups.\
  \ It\n    opens that follow-up only. GET calls also take it as ?token= (the links in our emails carry\n    one). A session signed in on licium.ai with the follow-up's email opens it too; an email\n    address alone never does.\n  sources:\n  - openapi/licium-ai-openapi.json\n- name: ReportDeleteCredential\n  type: apiKey\n  in: header\n  parameter: X-Licium-Report-Delete-Key\n  description: Anonymous report delete credential returned once by POST /v1/check when save=true.\n    Never put it in a URL.\n  sources:\n  - openapi/licium-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/licium-ai/authentication/licium-ai-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Company
- Healthcare
- Software-as-a-Service
- Credentialing
- Automation
---
