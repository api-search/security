---
api_key_in:
- header
api_specs:
- filename: levelblue-usm-anywhere-openapi.yml
  format: yaml
  label: USM Anywhere API
  slug: usm-anywhere-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/levelblue/refs/heads/main/openapi/levelblue-usm-anywhere-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Levelblue Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: LevelBlue secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: LevelBlue
provider_slug: levelblue
scheme_count: 2
schemes:
- applies_to:
  - POST /oauth/token
  detail: Client ID as the username, client secret as the password. Used only to obtain a token.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/levelblue-usm-anywhere-openapi.yml
  type: http
- applies_to:
  - all operations except POST /oauth/token
  bearerFormat: JWT
  default: true
  detail: 'Root-level security requirement — sent as Authorization: Bearer <access_token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/levelblue-usm-anywhere-openapi.yml
  type: http
slug: levelblue-authentication
source_filename: levelblue-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/levelblue-usm-anywhere-openapi.yml\ndocs: https://docs.levelblue.com/documentation/usm-anywhere/user-guide/user-management/api-clients\n\nsummary:\n  types: [http]\n  http_schemes: [basic, bearer]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  note: >-\n    The docs state \"USM Anywhere uses OAuth 2.0 to authenticate against the REST APIs\",\n    but the published spec models the exchange with plain http securitySchemes (basic on\n    the token endpoint, bearer everywhere else) rather than an oauth2 securityScheme with\n    a clientCredentials flow object.\n\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources: [openapi/levelblue-usm-anywhere-openapi.yml]\n  applies_to: ['POST /oauth/token']\n  detail: >-\n    Client ID as the username, client secret as the password. Used only to obtain a token.\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources: [openapi/levelblue-usm-anywhere-openapi.yml]\n\
  \  applies_to: [all operations except POST /oauth/token]\n  default: true\n  detail: 'Root-level security requirement — sent as Authorization: Bearer <access_token>.'\n\ntoken_exchange:\n  endpoint: POST /oauth/token\n  base_url_template: https://<subdomain>.alienvault.cloud/api/2.0\n  grant_type: client_credentials\n  request_content_type: application/x-www-form-urlencoded\n  client_authentication: http-basic\n  response:\n    access_token: JWT\n    token_type: bearer\n    expires_in: 899\n    scope: trust read write\n    jti: token identifier\n  failure: 401 Unauthorized (ErrorResponse envelope)\n\ncredential_provisioning:\n  ui_path: Profile Settings > API Clients\n  minimum_role: Manager\n  actions: [create client, enable/disable client, edit client ID]\n  detail: >-\n    Client credentials are created in the USM Anywhere web UI, not through an API. A newly\n    created client must be explicitly toggled enabled before it can obtain a token.\n  docs: https://docs.levelblue.com/documentation/usm-anywhere/user-guide/user-management/api-clients\n\
  \nauthorization:\n  model: role-based\n  roles: [Read-Only, Investigator, Analyst, Manager]\n  note: >-\n    Effective permissions follow the USM Anywhere role attached to the API client rather\n    than a requestable scope subset. See scopes/levelblue-scopes.yml.\n\nsecondary_surfaces:\n- name: USM Anywhere webhook ingestion\n  type: apiKey\n  in: header\n  parameter_name: API_KEY\n  also_accepted_in: query\n  endpoint: 'POST https://<base_url>/api/1.0/webhook/push'\n  rotatable: true\n  docs: https://docs.levelblue.com/documentation/usm-anywhere/user-guide/cloud-connector/webhook_connector/reset_api_key\n- name: LevelBlue Open Threat Exchange (OTX) DirectConnect API\n  type: apiKey\n  base_url: https://otx.alienvault.com/api/v1\n  validation_endpoint: /api/v1/users/me\n  docs: https://otx.alienvault.com/assets/static/external_api.html\n\nadditional_controls:\n  multifactor_authentication:\n    supported: true\n    scope: web UI sign-in (can be required tenant-wide); not applicable to\
  \ API clients\n    docs: https://docs.levelblue.com/documentation/usm-anywhere/user-guide/introduction/multifactor-authentication\n  single_sign_on:\n    supported: true\n    scope: web UI sign-in via SAML SSO configuration; not applicable to API clients\n    docs: https://docs.levelblue.com/documentation/usm-anywhere/user-guide/user-management/configuring-sso\n\ngaps:\n- No mutualTLS, openIdConnect or OIDC discovery document is published.\n- No token revocation or introspection endpoint is documented.\n- No refresh token is issued — clients re-run the client_credentials exchange.\n- The REST API is available only in the Standard and Premium editions of USM Anywhere.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/levelblue/refs/heads/main/authentication/levelblue-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Enterprise
- Cybersecurity
- Security
- Threat Intelligence
- Managed Security
- SIEM
- Threat Detection
- Incident Response
- Compliance
---
