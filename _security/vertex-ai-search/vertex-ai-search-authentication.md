---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: vertex-ai-search-projects-api-openapi.yml
  format: yaml
  label: Discovery Engine API (Vertex AI Search) - Projects
  slug: vertex-ai-search-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vertex-ai-search/openapi/vertex-ai-search-projects-api-openapi.yml
- filename: vertex-ai-search-billingaccounts-api-openapi.yml
  format: yaml
  label: Vertex AI Search Billing Accounts API
  slug: vertex-ai-search-billingaccounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vertex-ai-search/openapi/vertex-ai-search-billingaccounts-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Vertex AI Search Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Vertex AI Search secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Vertex AI Search
provider_slug: vertex-ai-search
scheme_count: 2
schemes:
- description: API key; accepted by methods that do not need user data.
  in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/vertex-ai-search-billing-accounts-api-openapi.yml
  - openapi/vertex-ai-search-projects-api-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/vertex-ai-search-billing-accounts-api-openapi.yml
  - openapi/vertex-ai-search-projects-api-openapi.yml
  type: oauth2
slug: vertex-ai-search-authentication
source_filename: vertex-ai-search-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/vertex-ai-search-billing-accounts-api-openapi.yml, openapi/vertex-ai-search-projects-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  description: API key; accepted by methods that do not need user data.\n  sources:\n  - openapi/vertex-ai-search-billing-accounts-api-openapi.yml\n  - openapi/vertex-ai-search-projects-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 5\n  sources:\n  - openapi/vertex-ai-search-billing-accounts-api-openapi.yml\n  - openapi/vertex-ai-search-projects-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/vertex-ai-search/authentication/vertex-ai-search-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- Search
- Enterprise
- Google Cloud
---
