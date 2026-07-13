---
api_key_in: []
api_specs:
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Companies API
  slug: simpro-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Customers API
  slug: simpro-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Sites API
  slug: simpro-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Jobs API
  slug: simpro-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Quotes API
  slug: simpro-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Invoices API
  slug: simpro-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Schedules API
  slug: simpro-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Vendor Orders API
  slug: simpro-vendor-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Cost Centers API
  slug: simpro-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Stock API
  slug: simpro-stock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
- filename: simpro-openapi.yml
  format: yaml
  label: Simpro Webhooks API
  slug: simpro-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/openapi/simpro-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Simpro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Simpro secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Simpro
provider_slug: simpro
scheme_count: 1
schemes:
- authorizationUrl: https://{build}.simprosuite.com/oauth2/authorize
  description: 'Simpro authenticates API applications with OAuth2 on the customer''s own build. An account administrator registers an API application on the build and issues client credentials. The integration then requests an access token from https://{build}.simprosuite.com/oauth2/token - using the same build subdomain that staff use to log in to the Simpro portal - and passes it as `Authorization: Bearer ACCESS_TOKEN` on every request. Both the client credentials grant and the authorization code grant are supported, depending on how the application is registered. There is no global or self-service API host; credentials and tokens are always scoped to a specific build.'
  flows:
  - clientCredentials
  - authorizationCode
  name: oauth2
  scheme: bearer
  sources:
  - openapi/simpro-openapi.yml
  - https://helpguide.simprogroup.com/Content/Service-and-Enterprise/API-FAQs.htm
  - https://apiforum.simprogroup.com/
  tokenUrl: https://{build}.simprosuite.com/oauth2/token
  type: oauth2
slug: simpro-authentication
source_filename: simpro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/simpro-openapi.yml\nsummary:\n  types:\n  - oauth2\nschemes:\n- name: oauth2\n  type: oauth2\n  scheme: bearer\n  description: >-\n    Simpro authenticates API applications with OAuth2 on the customer's own\n    build. An account administrator registers an API application on the build\n    and issues client credentials. The integration then requests an access\n    token from https://{build}.simprosuite.com/oauth2/token - using the same\n    build subdomain that staff use to log in to the Simpro portal - and passes\n    it as `Authorization: Bearer ACCESS_TOKEN` on every request. Both the\n    client credentials grant and the authorization code grant are supported,\n    depending on how the application is registered. There is no global or\n    self-service API host; credentials and tokens are always scoped to a\n    specific build.\n  flows:\n  - clientCredentials\n  - authorizationCode\n  tokenUrl: https://{build}.simprosuite.com/oauth2/token\n\
  \  authorizationUrl: https://{build}.simprosuite.com/oauth2/authorize\n  sources:\n  - openapi/simpro-openapi.yml\n  - https://helpguide.simprogroup.com/Content/Service-and-Enterprise/API-FAQs.htm\n  - https://apiforum.simprogroup.com/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpro/refs/heads/main/authentication/simpro-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Field Service Management
- Trades
- Job Management
- Project Management
- Scheduling
- Inventory
- Estimating
- Workforce
- SaaS
- Contractors
---
