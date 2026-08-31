---
api_key_in: []
api_specs:
- filename: ritten-calendar-api-openapi.yml
  format: yaml
  label: Ritten Calendar API
  slug: ritten-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-calendar-api-openapi.yml
- filename: ritten-cases-api-openapi.yml
  format: yaml
  label: Ritten Cases API
  slug: ritten-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-cases-api-openapi.yml
- filename: ritten-contacts-api-openapi.yml
  format: yaml
  label: Ritten Contacts API
  slug: ritten-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-contacts-api-openapi.yml
- filename: ritten-encounters-api-openapi.yml
  format: yaml
  label: Ritten Encounters API
  slug: ritten-encounters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-encounters-api-openapi.yml
- filename: ritten-facilities-api-openapi.yml
  format: yaml
  label: Ritten Facilities API
  slug: ritten-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-facilities-api-openapi.yml
- filename: ritten-forms-api-openapi.yml
  format: yaml
  label: Ritten Forms API
  slug: ritten-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-forms-api-openapi.yml
- filename: ritten-insights-api-openapi.yml
  format: yaml
  label: Ritten Insights API
  slug: ritten-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-insights-api-openapi.yml
- filename: ritten-insurance-api-openapi.yml
  format: yaml
  label: Ritten Insurance API
  slug: ritten-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-insurance-api-openapi.yml
- filename: ritten-oauth-api-openapi.yml
  format: yaml
  label: Ritten OAUTH API
  slug: ritten-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-oauth-api-openapi.yml
- filename: ritten-organizations-api-openapi.yml
  format: yaml
  label: Ritten Organizations API
  slug: ritten-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-organizations-api-openapi.yml
- filename: ritten-patients-api-openapi.yml
  format: yaml
  label: Ritten Patients API
  slug: ritten-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-patients-api-openapi.yml
- filename: ritten-programs-api-openapi.yml
  format: yaml
  label: Ritten Programs API
  slug: ritten-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-programs-api-openapi.yml
- filename: ritten-tasks-api-openapi.yml
  format: yaml
  label: Ritten Tasks API
  slug: ritten-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-tasks-api-openapi.yml
- filename: ritten-users-api-openapi.yml
  format: yaml
  label: Ritten Users API
  slug: ritten-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-users-api-openapi.yml
- filename: ritten-webhooks-api-openapi.yml
  format: yaml
  label: Ritten Webhooks API
  slug: ritten-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/openapi/ritten-webhooks-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ritten Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Ritten secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Ritten
provider_slug: ritten
scheme_count: 2
schemes:
- audience: https://external-api.ritten.io
  credentials:
  - client_id
  - client_secret
  flow: clientCredentials
  issuer: Auth0 (fronted by a Ritten caching proxy at /v1/oauth/token)
  name: OAuth2ClientCredentials
  request:
    body:
      audience: https://external-api.ritten.io
      client_id: ${client_id}
      client_secret: ${client_secret}
      grant_type: client_credentials
    content_type: application/json
    method: POST
  scopes: []
  scopes_note: No OAuth scopes are published. Access is provisioned per-integration by Ritten (e.g. CRM/organization access must be explicitly granted), not selected by scope at token time.
  sources:
  - https://docs.ritten.io/swagger/openapi.yaml
  token_lifetime_seconds: 86400
  token_url: https://api.ritten.io/v1/oauth/token
  type: oauth2
- description: The access_token from the token endpoint is sent as the Bearer token on every non-token request.
  name: BearerAuth
  scheme: bearer
  sources:
  - https://docs.ritten.io/swagger/openapi.yaml
  type: http
slug: ritten-authentication
source_filename: ritten-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: https://docs.ritten.io/swagger/openapi.yaml\ndocs: https://docs.ritten.io/\nnote: 'Ritten declares NO components.securitySchemes in its OpenAPI, so the mechanical derive finds nothing.\n  The auth model below is transcribed from the provider-published documentation in the spec info.description\n  (rendered at https://docs.ritten.io/). This is a real spec gap worth reporting to Ritten: the contract\n  is not self-describing for auth.'\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\n  declared_in_spec: false\n  documented_in_prose: true\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.ritten.io/v1/oauth/token\n  audience: https://external-api.ritten.io\n  credentials:\n  - client_id\n  - client_secret\n  request:\n    method: POST\n    content_type: application/json\n    body:\n      client_id: ${client_id}\n  \
  \    client_secret: ${client_secret}\n      audience: https://external-api.ritten.io\n      grant_type: client_credentials\n  token_lifetime_seconds: 86400\n  issuer: Auth0 (fronted by a Ritten caching proxy at /v1/oauth/token)\n  scopes: []\n  scopes_note: No OAuth scopes are published. Access is provisioned per-integration by Ritten (e.g. CRM/organization\n    access must be explicitly granted), not selected by scope at token time.\n  sources:\n  - https://docs.ritten.io/swagger/openapi.yaml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: The access_token from the token endpoint is sent as the Bearer token on every non-token\n    request.\n  sources:\n  - https://docs.ritten.io/swagger/openapi.yaml\nadditional_required_headers:\n- name: X-Ritten-Tenant\n  required: true\n  description: Selects the Ritten clinic instance the request targets. Required on every request.\n  example: ritclinic\nenvironments:\n- name: production\n  token_url: https://api.ritten.io/v1/oauth/token\n\
  \  audience: https://external-api.ritten.io\n  base_url: https://api.ritten.io/v1\n- name: beta\n  token_url: https://api.beta.ritten.io/v1/oauth/token\n  audience: https://external-api.beta.ritten.io\naccess_model:\n  self_service: false\n  note: Credentials are issued by Ritten to integrating partners; there is no public self-service signup\n    for API credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ritten/refs/heads/main/authentication/ritten-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Behavioral Health
- EMR
- EHR
- Healthcare
- Practice Management
- HIPAA
- Revenue Cycle Management
- Clinical Documentation
- Telehealth
- OpenAPI
- Webhook
- Behavioral Health API
- Substance Use Treatment
- 42 CFR Part 2
- Electronic Health Records
---
