---
api_key_in: []
api_specs:
- filename: logto-openapi-original.yml
  format: yaml
  label: Logto API
  slug: logto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logto/refs/heads/main/openapi/logto-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Logto Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Logto secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Logto
provider_slug: logto
scheme_count: 1
schemes:
- description: 'Logto Management API is a comprehensive set of REST APIs that gives you the full control over Logto to suit your product needs and tech stack. To see the full guide on Management API interactions, visit [Interact with Management API](https://docs.logto.io/docs/recipes/interact-with-management-api/).


    ### Get started


    The API follows the same authentication principles as other API resources in Logt'
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: /oidc/token
  name: OAuth2
  sources:
  - openapi/logto-openapi-original.yml
  type: oauth2
slug: logto-authentication
source_filename: logto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/logto-openapi-original.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oidc/token\n    scopes: 1\n  description: |-\n    Logto Management API is a comprehensive set of REST APIs that gives you the full control over Logto to suit your product needs and tech stack. To see the full guide on Management API interactions, visit [Interact with Management API](https://docs.logto.io/docs/recipes/interact-with-management-api/).\n\n    ### Get started\n\n    The API follows the same authentication principles as other API resources in Logt\n  sources:\n  - openapi/logto-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logto/refs/heads/main/authentication/logto-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Authentication
- Authorization
- Identity
- OIDC
- OAuth
- SAML
- Open Source
---
