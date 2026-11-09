---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dillilabs-com-analyze-api-openapi.yml
  format: yaml
  label: Dilli Labs Analyze API
  slug: dillilabs-com-analyze-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dillilabs-com/openapi/dillilabs-com-analyze-api-openapi.yml
- filename: dillilabs-com-health-api-openapi.yml
  format: yaml
  label: Dilli Labs Health API
  slug: dillilabs-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dillilabs-com/openapi/dillilabs-com-health-api-openapi.yml
- filename: dillilabs-com-privacy-api-openapi.yml
  format: yaml
  label: Dilli Labs Privacy API
  slug: dillilabs-com-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dillilabs-com/openapi/dillilabs-com-privacy-api-openapi.yml
- filename: dillilabs-com-purchase-api-openapi.yml
  format: yaml
  label: Dilli Labs Purchase API
  slug: dillilabs-com-purchase-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dillilabs-com/openapi/dillilabs-com-purchase-api-openapi.yml
- filename: dillilabs-com-user-api-openapi.yml
  format: yaml
  label: Dilli Labs User API
  slug: dillilabs-com-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dillilabs-com/openapi/dillilabs-com-user-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dillilabs Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dilli Labs declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Dilli Labs
provider_slug: dillilabs-com
scheme_count: 2
schemes:
- applies_to:
  - DEVA
  - DIL
  - DIVA
  - DeVIL
  description: REST APIs embed the API key as a path segment, e.g. GET https://deva.dillilabs.com/api/{API_KEY}/email/{address}, GET https://api.dillilabs.com/dil/<API_KEY>/ip/IP_ADDRESS, GET https://api.dillilabs.com/diva/<API_KEY>/ip/IP_ADDRESS, POST https://api.dillilabs.com/devil/{API_KEY}.
  in: path
  name: path-api-key
  type: apiKey
- applies_to:
  - DEVA MCP server
  description: 'MCP server https://deva.dillilabs.com/mcp (Streamable HTTP): "Authentication: API Key passed as X-DEVA-API-KEY header. Can be obtained from https://deva.dillilabs.com/register."'
  in: header
  name: X-DEVA-API-KEY
  type: apiKey
slug: dillilabs-com-authentication
source_filename: dillilabs-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://www.dillilabs.com/products/email-validation-api/\ndocs: https://www.dillilabs.com/products/email-validation-api/\nschemes:\n- name: path-api-key\n  type: apiKey\n  in: path\n  description: REST APIs embed the API key as a path segment, e.g. GET https://deva.dillilabs.com/api/{API_KEY}/email/{address}, GET https://api.dillilabs.com/dil/<API_KEY>/ip/IP_ADDRESS, GET https://api.dillilabs.com/diva/<API_KEY>/ip/IP_ADDRESS, POST https://api.dillilabs.com/devil/{API_KEY}.\n  applies_to: [DEVA, DIL, DIVA, DeVIL]\n- name: X-DEVA-API-KEY\n  type: apiKey\n  in: header\n  description: 'MCP server https://deva.dillilabs.com/mcp (Streamable HTTP): \"Authentication: API Key passed as X-DEVA-API-KEY header. Can be obtained from https://deva.dillilabs.com/register.\"'\n  applies_to: [DEVA MCP server]\nkey_issuance: DEVA keys via sign-up at https://deva.dillilabs.com/register; DIL, DIVA and DeVIL keys requested via a contact form on\
  \ each product page.\nnote: The Mind Your Tongue OpenAPI (openapi/_original/mindyourtongue-openapi.json) declares no securitySchemes; its operations are keyed by a device_id path parameter.\n"
source_yaml_url: https://artifacts.apis.io/dillilabs-com/authentication/dillilabs-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Email Verification
- IP Geolocation
- IP Validation
- Profanity Detection
- MCP
- Software-as-a-Service
- Web Hosting
- Software Development
---
