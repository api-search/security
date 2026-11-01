---
anonymous_access: false
api_key_in: []
api_specs:
- filename: recruitmcp-com-account-api-openapi.yml
  format: yaml
  label: recruitmcp-com Account API
  slug: recruitmcp-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-account-api-openapi.yml
- filename: recruitmcp-com-billing-api-openapi.yml
  format: yaml
  label: recruitmcp-com Billing API
  slug: recruitmcp-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-billing-api-openapi.yml
- filename: recruitmcp-com-companies-api-openapi.yml
  format: yaml
  label: recruitmcp-com Companies API
  slug: recruitmcp-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-companies-api-openapi.yml
- filename: recruitmcp-com-contacts-api-openapi.yml
  format: yaml
  label: recruitmcp-com Contacts API
  slug: recruitmcp-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-contacts-api-openapi.yml
- filename: recruitmcp-com-customers-api-openapi.yml
  format: yaml
  label: recruitmcp-com Customers API
  slug: recruitmcp-com-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-customers-api-openapi.yml
- filename: recruitmcp-com-events-api-openapi.yml
  format: yaml
  label: recruitmcp-com Events API
  slug: recruitmcp-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-events-api-openapi.yml
- filename: recruitmcp-com-lists-api-openapi.yml
  format: yaml
  label: recruitmcp-com Lists API
  slug: recruitmcp-com-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-lists-api-openapi.yml
- filename: recruitmcp-com-privacy-api-openapi.yml
  format: yaml
  label: recruitmcp-com Privacy API
  slug: recruitmcp-com-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-privacy-api-openapi.yml
- filename: recruitmcp-com-profiles-api-openapi.yml
  format: yaml
  label: recruitmcp-com Profiles API
  slug: recruitmcp-com-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-profiles-api-openapi.yml
- filename: recruitmcp-com-search-api-openapi.yml
  format: yaml
  label: recruitmcp-com Search API
  slug: recruitmcp-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/recruitmcp-com/openapi/recruitmcp-com-search-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Recruitmcp Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: recruitmcp-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: recruitmcp-com
provider_slug: recruitmcp-com
scheme_count: 2
schemes:
- description: API key (rmcp_live_…) or OAuth token (rmcp_oat_…).
  name: bearerAuth
  scheme: bearer
  type: http
- description: Authorization code with PKCE (S256).
  flows:
    authorizationCode:
      authorizationUrl: https://recruitmcp.com/oauth/authorize
      tokenUrl: https://recruitmcp.com/oauth/token
  name: oauth2
  type: oauth2
slug: recruitmcp-com-authentication
source_filename: recruitmcp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://recruitmcp.com/openapi.yaml\nschemes:\n  - type: http\n    scheme: bearer\n    name: bearerAuth\n    description: \"API key (rmcp_live_…) or OAuth token (rmcp_oat_…).\"\n  - type: oauth2\n    name: oauth2\n    description: \"Authorization code with PKCE (S256).\"\n    flows:\n      authorizationCode:\n        authorizationUrl: https://recruitmcp.com/oauth/authorize\n        tokenUrl: https://recruitmcp.com/oauth/token\n"
source_yaml_url: https://artifacts.apis.io/recruitmcp-com/authentication/recruitmcp-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Recruitment
- API
- MCP
- HR
---
