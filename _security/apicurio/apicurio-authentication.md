---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Apicurio Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Apicurio secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Apicurio
provider_slug: apicurio
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/apicurio-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://example.com/realms/apicurio/protocol/openid-connect/token
  name: OAuth2
  sources:
  - openapi/apicurio-openapi.yml
  type: oauth2
slug: apicurio-authentication
source_filename: apicurio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apicurio-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/apicurio-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/realms/apicurio/protocol/openid-connect/token\n    scopes: 3\n  sources:\n  - openapi/apicurio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apicurio/refs/heads/main/authentication/apicurio-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Apache License
- API Design
- API Registry
- Avro
- AsyncAPI
- Java
- Open Source
- OpenAPI
- Red Hat
- Schema Registry
---
