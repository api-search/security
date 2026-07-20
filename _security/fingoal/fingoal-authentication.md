---
api_key_in: []
api_specs:
- filename: fingoal-insights-openapi-original.json
  format: json
  label: FinGoal Insights API
  slug: fingoal-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fingoal/refs/heads/main/openapi/fingoal-insights-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Fingoal Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: FinGoal secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: FinGoal
provider_slug: fingoal
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://findmoney.fingoal.com/v3/authentication
  name: Authentication
  sources:
  - openapi/fingoal-insights-openapi-original.json
  type: oauth2
slug: fingoal-authentication
source_filename: fingoal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/fingoal-insights-openapi-original.json\ndocs: https://docs.fingoal.dev/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nnotes: >-\n  The Insights API is declared as OAuth2 clientCredentials in the OpenAPI, but\n  the token is minted by a custom endpoint: POST\n  https://findmoney.fingoal.com/v3/authentication with a JSON body\n  {\"client_id\",\"client_secret\"} returns a JWT `access_token`. That JWT is then\n  sent as `Authorization: Bearer <token>` on every request. Developer\n  credentials are issued on request (24h turnaround) via\n  https://fingoal.com/request-developer-account - there is no public self-serve\n  signup. Dev credentials target the findmoney-dev host; production the\n  findmoney host.\nschemes:\n- name: Authentication\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://findmoney.fingoal.com/v3/authentication\n    scopes: 1\n  sources:\n  - openapi/fingoal-insights-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fingoal/refs/heads/main/authentication/fingoal-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Financial Services
- Fintech
- Transaction Enrichment
- Data Enrichment
- Personal Financial Management
- Banking
- Categorization
- Webhooks
---
