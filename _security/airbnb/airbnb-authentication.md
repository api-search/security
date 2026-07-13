---
api_key_in: []
api_specs:
- filename: airbnb-homes-api-openapi.yml
  format: yaml
  label: Airbnb Homes API
  slug: homes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/openapi/airbnb-homes-api-openapi.yml
- filename: airbnb-activities-api-openapi.yml
  format: yaml
  label: Airbnb Activities API
  slug: activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/openapi/airbnb-activities-api-openapi.yml
- filename: airbnb-webhooks-asyncapi.yml
  format: yaml
  label: Airbnb Webhooks API
  slug: webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/asyncapi/airbnb-webhooks-asyncapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Airbnb Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: airbnb secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: airbnb
provider_slug: airbnb
scheme_count: 1
schemes:
- description: Airbnb uses OAuth 2.0 for authentication. Partners must register their application to receive a client ID and secret, then obtain access tokens through the authorization code flow.
  flows:
  - authorizationUrl: https://www.airbnb.com/oauth2/auth
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://api.airbnb.com/v2/oauth2/authorizations
  name: oauth2
  sources:
  - openapi/airbnb-activities-api-openapi.yml
  - openapi/airbnb-homes-api-openapi.yml
  type: oauth2
slug: airbnb-authentication
source_filename: airbnb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/airbnb-activities-api-openapi.yml, openapi/airbnb-homes-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.airbnb.com/oauth2/auth\n    tokenUrl: https://api.airbnb.com/v2/oauth2/authorizations\n    scopes: 6\n  description: Airbnb uses OAuth 2.0 for authentication. Partners must register their application\n    to receive a client ID and secret, then obtain access tokens through the authorization code\n    flow.\n  sources:\n  - openapi/airbnb-activities-api-openapi.yml\n  - openapi/airbnb-homes-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airbnb/refs/heads/main/authentication/airbnb-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
