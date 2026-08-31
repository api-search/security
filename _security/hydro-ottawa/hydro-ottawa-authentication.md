---
api_key_in: []
api_specs:
- filename: hydro-ottawa-applicationinformation-api-openapi.yml
  format: yaml
  label: Hydro Ottawa Application Information API
  slug: hydro-ottawa-applicationinformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/openapi/hydro-ottawa-applicationinformation-api-openapi.yml
- filename: hydro-ottawa-authorization-api-openapi.yml
  format: yaml
  label: Hydro Ottawa Authorization API
  slug: hydro-ottawa-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/openapi/hydro-ottawa-authorization-api-openapi.yml
- filename: hydro-ottawa-batch-api-openapi.yml
  format: yaml
  label: Hydro Ottawa Batch API
  slug: hydro-ottawa-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/openapi/hydro-ottawa-batch-api-openapi.yml
- filename: hydro-ottawa-usagepoint-api-openapi.yml
  format: yaml
  label: Hydro Ottawa Usage Point API
  slug: hydro-ottawa-usagepoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/openapi/hydro-ottawa-usagepoint-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Hydro Ottawa Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Hydro Ottawa secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Hydro Ottawa
provider_slug: hydro-ottawa
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  sources:
  - openapi/hydro-ottawa-green-button-espi-openapi.yml
  type: oauth2
slug: hydro-ottawa-authentication
source_filename: hydro-ottawa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/hydro-ottawa-green-button-espi-openapi.yml\nnote: >-\n  The source specification is authored by the Green Button Alliance, not by Hydro Ottawa,\n  and the authorizationUrl and tokenUrl below belong to the GBA sandbox. Hydro Ottawa\n  publishes no OAuth endpoints, no scope reference and no anonymously served OpenID Connect\n  discovery document (see well-known/hydro-ottawa-well-known.yml). Hydro Ottawa's own\n  description of Connect My Data — third party initiates, customer is redirected into Hydro\n  Ottawa's Green Button authentication, customer selects data types, duration and frequency\n  and may revoke at any time — matches the authorization-code model recorded here, but the\n  concrete endpoints were NOT observed and none were invented. The customer-facing half of\n  the flow is live at https://hydroottawa.savagedata.com/Connect/Authorize.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n\
  \  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n    scopes: 0\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n    scopes: 0\n  sources:\n  - openapi/hydro-ottawa-green-button-espi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydro-ottawa/refs/heads/main/authentication/hydro-ottawa-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Energy
- Canada
- Ontario
- Utilities
- Electricity
- Electricity Distribution
- Smart Metering
- Green Button
- ESPI
- Municipal Utility
- Renewables
- Hydroelectric
- Solar
- Demand Response
- Grid
---
