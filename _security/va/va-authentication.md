---
api_key_in:
- cookie
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Benefits Intake API
  slug: benefits-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/department-of-veterans-affairs/vets-api-clients/master/services/benefits-intake/openapi.yaml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Va Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Veterans Affairs secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Veterans Affairs
provider_slug: va
scheme_count: 5
schemes:
- bearerFormat: JWT
  name: bearer_token
  scheme: bearer
  sources:
  - openapi/va-appealable-issues-openapi.json
  - openapi/va-appeals-status-openapi.json
  - openapi/va-claims-api-openapi.json
  - openapi/va-higher-level-reviews-openapi.json
  - openapi/va-legacy-appeals-openapi.json
  - openapi/va-notice-of-disagreements-openapi.json
  - openapi/va-supplemental-claims-openapi.json
  type: http
- description: 'The authentication model for the Appealable Issues API uses OAuth 2.0/OpenID Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/appealable-issues/authorization-code) and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/appealable-issues/client-credentials).'
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    scopes: 2
    tokenUrl: To get production access, you must either work for VA or have specific VA agreements in place. If you have questions, [contact us](https://developer.va.gov/support/contact-us).
  name: productionOauth
  sources:
  - openapi/va-appealable-issues-openapi.json
  - openapi/va-appeals-status-openapi.json
  - openapi/va-higher-level-reviews-openapi.json
  - openapi/va-legacy-appeals-openapi.json
  - openapi/va-notice-of-disagreements-openapi.json
  - openapi/va-supplemental-claims-openapi.json
  type: oauth2
- description: This API uses OAuth 2 with the client credential grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/client-credentials)
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/authorization
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.va.gov/oauth2/token
  name: productionOauth
  sources:
  - openapi/va-claims-api-openapi.json
  type: oauth2
- in: header
  name: apikey
  parameter: apikey
  sources:
  - openapi/va-decision-reviews-openapi.json
  type: apiKey
- description: An authenticated session is established using the Sessions Controller to initiate federated authentication with an external credential provider, after which an API session token is established in the api_session cookie.
  in: cookie
  name: CookieAuth
  parameter: api_session
  sources:
  - openapi/va-patient-health-openapi.yaml
  type: apiKey
slug: va-authentication
source_filename: va-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/va-appealable-issues-openapi.json, openapi/va-appeals-status-openapi.json, openapi/va-claims-api-openapi.json,\n  openapi/va-decision-reviews-openapi.json, openapi/va-higher-level-reviews-openapi.json, openapi/va-legacy-appeals-openapi.json,\n  openapi/va-notice-of-disagreements-openapi.json, openapi/va-patient-health-openapi.yaml, openapi/va-supplemental-claims-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: bearer_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/va-appealable-issues-openapi.json\n  - openapi/va-appeals-status-openapi.json\n  - openapi/va-claims-api-openapi.json\n  - openapi/va-higher-level-reviews-openapi.json\n  - openapi/va-legacy-appeals-openapi.json\n  - openapi/va-notice-of-disagreements-openapi.json\n  - openapi/va-supplemental-claims-openapi.json\n\
  - name: productionOauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token\n    scopes: 4\n  - flow: clientCredentials\n    tokenUrl: To get production access, you must either work for VA or have specific VA agreements\n      in place. If you have questions, [contact us](https://developer.va.gov/support/contact-us).\n    scopes: 2\n  description: 'The authentication model for the Appealable Issues API uses OAuth 2.0/OpenID\n    Connect. The following authorization models are supported: [Authorization code flow](https://developer.va.gov/explore/api/appealable-issues/authorization-code)\n    and [Client Credentials Grant (CCG)](https://developer.va.gov/explore/api/appealable-issues/client-credentials).'\n  sources:\n  - openapi/va-appealable-issues-openapi.json\n  - openapi/va-appeals-status-openapi.json\n  - openapi/va-higher-level-reviews-openapi.json\n\
  \  - openapi/va-legacy-appeals-openapi.json\n  - openapi/va-notice-of-disagreements-openapi.json\n  - openapi/va-supplemental-claims-openapi.json\n- name: productionOauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/authorization\n    tokenUrl: https://api.va.gov/oauth2/token\n    scopes: 2\n  description: This API uses OAuth 2 with the client credential grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/client-credentials)\n  sources:\n  - openapi/va-claims-api-openapi.json\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/va-decision-reviews-openapi.json\n- name: CookieAuth\n  type: apiKey\n  in: cookie\n  parameter: api_session\n  description: An authenticated session is established using the Sessions Controller to initiate\n    federated authentication with an external credential provider, after which an API session\n    token is established in the api_session\
  \ cookie.\n  sources:\n  - openapi/va-patient-health-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/va/refs/heads/main/authentication/va-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Veterans
- Government
- Health
- Benefits
- FHIR
- Appeals
- Federal
---
