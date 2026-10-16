---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cuebiq-conversion-feed-v1-api-openapi.yml
  format: yaml
  label: Cuebiq Conversion Feed V1 API
  slug: cuebiq-conversion-feed-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-conversion-feed-v1-api-openapi.yml
- filename: cuebiq-geoset-api-openapi.yml
  format: yaml
  label: Cuebiq Geoset API
  slug: cuebiq-geoset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-geoset-api-openapi.yml
- filename: cuebiq-kpis-v2-campaign-reports-api-openapi.yml
  format: yaml
  label: Cuebiq KPIs V2 - Campaign Reports API
  slug: cuebiq-kpis-v2-campaign-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-kpis-v2-campaign-reports-api-openapi.yml
- filename: cuebiq-kpis-v2-campaigns-api-openapi.yml
  format: yaml
  label: Cuebiq KPIs V2 - Campaigns API
  slug: cuebiq-kpis-v2-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-kpis-v2-campaigns-api-openapi.yml
- filename: cuebiq-kpis-v2-customer-api-openapi.yml
  format: yaml
  label: Cuebiq KPIs V2 - Customer API
  slug: cuebiq-kpis-v2-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-kpis-v2-customer-api-openapi.yml
- filename: cuebiq-kpis-v2-shared-campaign-reports-api-openapi.yml
  format: yaml
  label: Cuebiq KPIs V2 - Shared Campaign Reports API
  slug: cuebiq-kpis-v2-shared-campaign-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-kpis-v2-shared-campaign-reports-api-openapi.yml
- filename: cuebiq-kpis-v2-shared-campaigns-api-openapi.yml
  format: yaml
  label: Cuebiq KPIs V2 - Shared Campaigns API
  slug: cuebiq-kpis-v2-shared-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-kpis-v2-shared-campaigns-api-openapi.yml
- filename: cuebiq-kpis-v2-shared-reports-api-openapi.yml
  format: yaml
  label: Cuebiq KPIs V2 - Shared Reports API
  slug: cuebiq-kpis-v2-shared-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-kpis-v2-shared-reports-api-openapi.yml
- filename: cuebiq-measurement-v2-api-openapi.yml
  format: yaml
  label: Cuebiq Measurement V2 API
  slug: cuebiq-measurement-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/openapi/cuebiq-measurement-v2-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cuebiq Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Cuebiq secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Cuebiq
provider_slug: cuebiq
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.cuebiq.com/auth/realms/Customers/protocol/openid-connect/token
  name: cuebiq_auth
  sources:
  - openapi/cuebiq-openapi.json
  type: oauth2
slug: cuebiq-authentication
source_filename: cuebiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: derived\nsource: openapi/cuebiq-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: cuebiq_auth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.cuebiq.com/auth/realms/Customers/protocol/openid-connect/token\n    scopes: 0\n  sources:\n  - openapi/cuebiq-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuebiq/refs/heads/main/authentication/cuebiq-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Location-Intelligence
- Marketing
- Data-Analytics
- Footfall-Measurement
---
