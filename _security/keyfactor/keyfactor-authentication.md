---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Keyfactor Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- password
overview: Keyfactor secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and password flow(s).
provider_name: Keyfactor
provider_slug: keyfactor
scheme_count: 2
schemes:
- description: Active Directory service-account authentication (HTTP Basic or Windows integrated authentication) against a Keyfactor Command instance.
  name: activeDirectoryBasic
  scheme: basic
  type: http
- description: 'OAuth 2.0 client-credentials grant via an OIDC identity provider (Keycloak or equivalent). Access token is sent as `Authorization: Bearer <token>`. Password grant is also supported for development scenarios.'
  flow: clientCredentials
  name: oauth2ClientCredentials
  type: oauth2
slug: keyfactor-authentication
source_filename: keyfactor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://software.keyfactor.com/Core-OnPrem/Current/Content/WebAPI/AuthenticateAPI.htm\ndocs: https://software.keyfactor.com/Core-OnPrem/Current/Content/WebAPI/AuthenticateAPI.htm\nsummary:\n  types: [http, oauth2]\n  api_key_in: []\n  oauth2_flows: [clientCredentials, password]\n  scope: >-\n    Keyfactor Command Web API. EJBCA REST API additionally supports client\n    (mutual-TLS) certificate authentication per deployment.\nschemes:\n  - name: activeDirectoryBasic\n    type: http\n    scheme: basic\n    description: >-\n      Active Directory service-account authentication (HTTP Basic or Windows\n      integrated authentication) against a Keyfactor Command instance.\n  - name: oauth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    description: >-\n      OAuth 2.0 client-credentials grant via an OIDC identity provider\n      (Keycloak or equivalent). Access token is sent as `Authorization: Bearer\n   \
  \   <token>`. Password grant is also supported for development scenarios.\nrequired_headers:\n  - name: x-keyfactor-requested-with\n    value: APIClient\n  - name: Authorization\n    value: Basic <creds> | Bearer <token>\n  - name: Accept\n    value: application/json\nnotes: >-\n  Keyfactor Command is self-hosted or Cloud PKI-as-a-Service; the specific\n  identity provider and token endpoints are configured per customer instance.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keyfactor/refs/heads/main/authentication/keyfactor-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Cybersecurity
- PKI
- Machine Identity
- Certificate Lifecycle
- Code Signing
- Cryptography
- Digital Trust
- Security
---
