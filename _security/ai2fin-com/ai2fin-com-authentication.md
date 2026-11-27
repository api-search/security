---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ai2fin-com-ai-analysis-api-openapi.yml
  format: yaml
  label: AI2Fin AI Analysis API
  slug: ai2fin-com-ai-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-ai-analysis-api-openapi.yml
- filename: ai2fin-com-ai-assistant-api-openapi.yml
  format: yaml
  label: AI2Fin AI Assistant API
  slug: ai2fin-com-ai-assistant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-ai-assistant-api-openapi.yml
- filename: ai2fin-com-ai-services-api-openapi.yml
  format: yaml
  label: AI2Fin AI Services API
  slug: ai2fin-com-ai-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-ai-services-api-openapi.yml
- filename: ai2fin-com-analytics-reports-api-openapi.yml
  format: yaml
  label: AI2Fin Analytics & Reports API
  slug: ai2fin-com-analytics-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-analytics-reports-api-openapi.yml
- filename: ai2fin-com-authentication-api-openapi.yml
  format: yaml
  label: AI2Fin Authentication API
  slug: ai2fin-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-authentication-api-openapi.yml
- filename: ai2fin-com-automation-api-openapi.yml
  format: yaml
  label: AI2Fin Automation API
  slug: ai2fin-com-automation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-automation-api-openapi.yml
- filename: ai2fin-com-bank-transactions-api-openapi.yml
  format: yaml
  label: AI2Fin Bank Transactions API
  slug: ai2fin-com-bank-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-bank-transactions-api-openapi.yml
- filename: ai2fin-com-bills-recurring-payments-api-openapi.yml
  format: yaml
  label: AI2Fin Bills & Recurring Payments API
  slug: ai2fin-com-bills-recurring-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-bills-recurring-payments-api-openapi.yml
- filename: ai2fin-com-categories-api-openapi.yml
  format: yaml
  label: AI2Fin Categories API
  slug: ai2fin-com-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-categories-api-openapi.yml
- filename: ai2fin-com-expenses-api-openapi.yml
  format: yaml
  label: AI2Fin Expenses API
  slug: ai2fin-com-expenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-expenses-api-openapi.yml
- filename: ai2fin-com-gst-tax-api-openapi.yml
  format: yaml
  label: AI2Fin GST & Tax API
  slug: ai2fin-com-gst-tax-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-gst-tax-api-openapi.yml
- filename: ai2fin-com-mcp-server-api-openapi.yml
  format: yaml
  label: AI2Fin MCP Server API
  slug: ai2fin-com-mcp-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-mcp-server-api-openapi.yml
- filename: ai2fin-com-receipts-attachments-api-openapi.yml
  format: yaml
  label: AI2Fin Receipts & Attachments API
  slug: ai2fin-com-receipts-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-receipts-attachments-api-openapi.yml
- filename: ai2fin-com-search-api-openapi.yml
  format: yaml
  label: AI2Fin Search API
  slug: ai2fin-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-search-api-openapi.yml
- filename: ai2fin-com-smart-categories-api-openapi.yml
  format: yaml
  label: AI2Fin Smart Categories API
  slug: ai2fin-com-smart-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-smart-categories-api-openapi.yml
- filename: ai2fin-com-subscription-api-openapi.yml
  format: yaml
  label: AI2Fin Subscription API
  slug: ai2fin-com-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-subscription-api-openapi.yml
- filename: ai2fin-com-travel-vehicles-api-openapi.yml
  format: yaml
  label: AI2Fin Travel & Vehicles API
  slug: ai2fin-com-travel-vehicles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai2fin-com/openapi/ai2fin-com-travel-vehicles-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: AI2Fin Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI2Fin declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AI2Fin
provider_slug: ai2fin-com
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: First-party access token for your own signed-in session, obtained from the /api/enterprise-auth/login endpoint.
  name: bearerAuth
  scheme: bearer
  type: http
- description: Session cookie for web applications
  in: cookie
  name: ai2_sess
  type: apiKey
slug: ai2fin-com-authentication
source_filename: ai2fin-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://docs.ai2fin.com/api-reference/authentication/login-user.md\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    name: bearerAuth\n    description: \"First-party access token for your own signed-in session, obtained from the /api/enterprise-auth/login endpoint.\"\n  - type: apiKey\n    in: cookie\n    name: ai2_sess\n    description: \"Session cookie for web applications\"\n"
source_yaml_url: https://artifacts.apis.io/ai2fin-com/authentication/ai2fin-com-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Tax
- Personal Finance
- Software-as-a-Service
- Employee Benefits
---
