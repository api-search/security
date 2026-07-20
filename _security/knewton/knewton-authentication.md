---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Knewton Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- refreshToken
overview: Knewton secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and refreshToken flow(s).
provider_name: Knewton
provider_slug: knewton
scheme_count: 2
schemes:
- caller: Partner admin user must make the token call.
  client_authentication: basic
  client_authentication_detail: 'Authorization: Basic <key>, where <key> is formed by base64 encoding <api_key>:<api_secret>'
  flow: clientCredentials
  grant_types:
  - client_credentials
  - refresh_token
  name: OAuth2ClientCredentials
  scope_parameter:
    description: On the client_credentials grant the scope parameter is not a permission scope. It carries the external ID of a previously created user account to be associated with the returned tokens.
    example_form: scope=user_601726
    semantics: external-user-id
    supported: true
  sources:
  - https://dev.knewton.com/reference/authentication/
  token_endpoint_path: /oauth/token
  token_lifetime:
    approximate: ~180 days
    expires_in_seconds: 15555599
    response_fields:
    - access_token
    - refresh_token
    - expires_in
    - expires_at
  token_url: https://api.knewton.com/v0/oauth/token
  type: oauth2
- description: All non-token endpoints accept the OAuth access token as a bearer credential. Only the /oauth/token endpoint uses Basic authentication with the partner API key and secret.
  name: BearerToken
  scheme: bearer
  sources:
  - https://dev.knewton.com/reference/authentication/
  type: http
slug: knewton-authentication
source_filename: knewton-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://dev.knewton.com/reference/authentication/\ndocs: https://dev.knewton.com/implementation/authentication-and-authorization/\ncredentials_docs: https://dev.knewton.com/implementation/partner-credentials/\nnote: Knewton publishes no OpenAPI definition; this profile is captured from the published\n  authentication reference rather than derived from a machine-readable spec.\nsummary:\n  types:\n  - oauth2\n  - http\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  - refreshToken\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.knewton.com/v0/oauth/token\n  token_endpoint_path: /oauth/token\n  client_authentication: basic\n  client_authentication_detail: 'Authorization: Basic <key>, where <key> is formed by base64\n    encoding <api_key>:<api_secret>'\n  grant_types:\n  - client_credentials\n  - refresh_token\n  scope_parameter:\n    supported: true\n\
  \    semantics: external-user-id\n    description: On the client_credentials grant the scope parameter is not a permission\n      scope. It carries the external ID of a previously created user account to be associated\n      with the returned tokens.\n    example_form: scope=user_601726\n  token_lifetime:\n    expires_in_seconds: 15555599\n    approximate: ~180 days\n    response_fields:\n    - access_token\n    - refresh_token\n    - expires_in\n    - expires_at\n  caller: Partner admin user must make the token call.\n  sources:\n  - https://dev.knewton.com/reference/authentication/\n- name: BearerToken\n  type: http\n  scheme: bearer\n  description: All non-token endpoints accept the OAuth access token as a bearer credential.\n    Only the /oauth/token endpoint uses Basic authentication with the partner API key and\n    secret.\n  sources:\n  - https://dev.knewton.com/reference/authentication/\ncredential_provisioning:\n  self_service: false\n  description: Each learning application\
  \ integrated with the Knewton API has a unique partner\n    client ID and secret provided by a Knewton representative. There is no public self-service\n    sign-up for API credentials.\n  docs: https://dev.knewton.com/implementation/partner-credentials/\nauthorization_model:\n  style: entitlements\n  description: Authorization is expressed as entitlements on an account, returned on\n    GET /accounts/{account_id}. Most write operations require the partner admin user;\n    read operations are permitted for the partner admin or the account/registration owner.\n  entitlements:\n  - all\n  - knerd\n  - partner_admin\n  - partner_inventory_access\n  - partner_graph_update\n  - partner_graph_ingest\n  - partner_graph_validate\n  - create_learning_instance\n  source: https://dev.knewton.com/reference/accounts/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knewton/refs/heads/main/authentication/knewton-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Consumer
- Education
- EdTech
- Adaptive Learning
- Learning Analytics
- Machine Learning
- Recommendations
- Courseware
- Higher Education
---
