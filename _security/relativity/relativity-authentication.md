---
api_key_in: []
api_specs:
- filename: relativity-object-manager-openapi.yml
  format: yaml
  label: Relativity Object Manager API
  slug: relativity-object-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-object-manager-openapi.yml
- filename: relativity-import-openapi.yml
  format: yaml
  label: Relativity Import Service API
  slug: relativity-import-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-import-openapi.yml
- filename: relativity-export-openapi.yml
  format: yaml
  label: Relativity Export Service API
  slug: relativity-export-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-export-openapi.yml
- filename: relativity-workspace-openapi.yml
  format: yaml
  label: Relativity Workspace Manager API
  slug: relativity-workspace-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-workspace-openapi.yml
- filename: relativity-productions-openapi.yml
  format: yaml
  label: Relativity Production Manager API
  slug: relativity-production-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-productions-openapi.yml
- filename: relativity-legal-hold-openapi.yml
  format: yaml
  label: Relativity Legal Hold API
  slug: relativity-legal-hold-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-legal-hold-openapi.yml
- filename: relativity-automated-workflows-openapi.yml
  format: yaml
  label: Relativity Automated Workflows API
  slug: relativity-automated-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-automated-workflows-openapi.yml
- filename: relativity-permissions-openapi.yml
  format: yaml
  label: Relativity Audit API
  slug: relativity-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-permissions-openapi.yml
- filename: relativity-identity-openapi.yml
  format: yaml
  label: Relativity User and Permission Manager API
  slug: relativity-user-and-permission-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-identity-openapi.yml
- filename: relativity-billing-v2-openapi.yml
  format: yaml
  label: Relativity Billing Insights API
  slug: relativity-billing-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/openapi/relativity-billing-v2-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Relativity Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Relativity secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Relativity
provider_slug: relativity
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'Relativity Identity Service (RIS) bearer token to authenticate: https://platform.relativity.com/RelativityOne/Content/REST_API/REST_API_authentication.htm#Bearertokenauthentication'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/relativity-collect-openapi.yml
  - openapi/relativity-permissions-openapi.yml
  - openapi/relativity-review-service-openapi.yml
  - openapi/relativity-staging-reports-openapi.yml
  - openapi/relativity-transfer-openapi.yml
  - openapi/relativity-usage-reports-openapi.yml
  - openapi/relativity-workspace-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.relone.preview.com/oauth/token
  name: oauth2
  sources:
  - openapi/relativity-glacier-openapi.yml
  type: oauth2
slug: relativity-authentication
source_filename: relativity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/relativity-collect-openapi.yml, openapi/relativity-glacier-openapi.yml, openapi/relativity-permissions-openapi.yml,\n  openapi/relativity-review-service-openapi.yml, openapi/relativity-staging-reports-openapi.yml,\n  openapi/relativity-transfer-openapi.yml, openapi/relativity-usage-reports-openapi.yml, openapi/relativity-workspace-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Relativity Identity Service (RIS) bearer token to authenticate: https://platform.relativity.com/RelativityOne/Content/REST_API/REST_API_authentication.htm#Bearertokenauthentication'\n  sources:\n  - openapi/relativity-collect-openapi.yml\n  - openapi/relativity-permissions-openapi.yml\n  - openapi/relativity-review-service-openapi.yml\n  - openapi/relativity-staging-reports-openapi.yml\n  - openapi/relativity-transfer-openapi.yml\n\
  \  - openapi/relativity-usage-reports-openapi.yml\n  - openapi/relativity-workspace-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.relone.preview.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/relativity-glacier-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relativity/refs/heads/main/authentication/relativity-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- eDiscovery
- Legal
- Document Review
- Legal Technology
- Data Processing
- AI Review
- Litigation
- Compliance
---
