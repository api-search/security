---
api_key_in: []
api_specs:
- filename: orbii-business-category-assignment-api-openapi.yml
  format: yaml
  label: Orbii Business Category Assignment API
  slug: orbii-business-category-assignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-business-category-assignment-api-openapi.yml
- filename: orbii-categories-api-openapi.yml
  format: yaml
  label: Orbii Categories API
  slug: orbii-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-categories-api-openapi.yml
- filename: orbii-clients-api-openapi.yml
  format: yaml
  label: Orbii Clients API
  slug: orbii-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-clients-api-openapi.yml
- filename: orbii-company-management-api-openapi.yml
  format: yaml
  label: Orbii Company Management API
  slug: orbii-company-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-company-management-api-openapi.yml
- filename: orbii-data-check-api-openapi.yml
  format: yaml
  label: Orbii Data Check API
  slug: orbii-data-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-data-check-api-openapi.yml
- filename: orbii-general-api-openapi.yml
  format: yaml
  label: Orbii General API
  slug: orbii-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-general-api-openapi.yml
- filename: orbii-ibans-api-openapi.yml
  format: yaml
  label: Orbii IBANs API
  slug: orbii-ibans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-ibans-api-openapi.yml
- filename: orbii-invoices-api-openapi.yml
  format: yaml
  label: Orbii Invoices API
  slug: orbii-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-invoices-api-openapi.yml
- filename: orbii-kpis-api-openapi.yml
  format: yaml
  label: Orbii KPIs API
  slug: orbii-kpis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-kpis-api-openapi.yml
- filename: orbii-lending-actions-api-openapi.yml
  format: yaml
  label: Orbii Lending Actions API
  slug: orbii-lending-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-lending-actions-api-openapi.yml
- filename: orbii-merchants-api-openapi.yml
  format: yaml
  label: Orbii Merchants API
  slug: orbii-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-merchants-api-openapi.yml
- filename: orbii-pdfs-api-openapi.yml
  format: yaml
  label: Orbii PDFs API
  slug: orbii-pdfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-pdfs-api-openapi.yml
- filename: orbii-risk-assessment-api-openapi.yml
  format: yaml
  label: Orbii Risk Assessment API
  slug: orbii-risk-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-risk-assessment-api-openapi.yml
- filename: orbii-subcategories-api-openapi.yml
  format: yaml
  label: Orbii Subcategories API
  slug: orbii-subcategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-subcategories-api-openapi.yml
- filename: orbii-transactions-api-openapi.yml
  format: yaml
  label: Orbii Transactions API
  slug: orbii-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-transactions-api-openapi.yml
auth_types:
- query-credentials
description: ''
kind: authentication
layout: security
method: searched
name: Orbii Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orbii secures its APIs with query-credentials across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Orbii
provider_slug: orbii
scheme_count: 1
schemes:
- applies_to: subset of endpoints (e.g. GET /clients)
  documented_in: openapi/orbii-uae-openapi-original.json
  location: query
  name: query-credentials
  parameters:
  - user
  - password
  - client
  type: custom
slug: orbii-authentication
source_filename: orbii-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/orbii-uae-openapi-original.json + api.docs.orbii.ai\nsummary:\n  types: [query-credentials]\n  declared_security_schemes: none\n  note: >-\n    The published OpenAPI specs declare no components.securitySchemes. Auth is\n    handled out-of-band / via credentials passed as query parameters on selected\n    endpoints (user, password) with a 'client' parameter scoping the lender.\nschemes:\n  - name: query-credentials\n    type: custom\n    location: query\n    parameters: [user, password, client]\n    applies_to: subset of endpoints (e.g. GET /clients)\n    documented_in: openapi/orbii-uae-openapi-original.json\nrecommendation: >-\n  Orbii should declare an apiKey or OAuth2 securityScheme and stop accepting\n  credentials in query strings (they leak into logs and browser history).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/authentication/orbii-authentication.yml
summary_line: query-credentials · 1 scheme
tags:
- Company
- Artificial Intelligence
- Lending
- Credit
- Fintech
- Underwriting
- Banking
- SME
- Embedded Finance
- MENA
- Risk
---
