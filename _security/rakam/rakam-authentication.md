---
api_key_in: []
auth_types:
- saml
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Rakam Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: rakam secures its APIs with saml, oauth2, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: rakam
provider_slug: rakam
scheme_count: 3
schemes:
- description: SAML 2.0 single sign-on for platform access (Enterprise plan).
  docs: https://docs.rakam.io/docs/saml-authentication
  name: SAML SSO
  type: saml
- description: GSuite / Google Workspace OAuth2 authentication for platform login.
  docs: https://docs.rakam.io/docs/google-oauth2-authentication
  flow: authorizationCode
  name: Google Workspace OAuth2
  type: oauth2
- description: The open-source rakam-api event-collection server authenticates ingest with project write/master API keys sent by the client SDKs.
  name: API key (event collection)
  source: https://github.com/rakam-io/rakam-api
  type: apiKey
slug: rakam-authentication
source_filename: rakam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.rakam.io/docs/saml-authentication, https://docs.rakam.io/docs/google-oauth2-authentication\nnote: >-\n  No committed OpenAPI/Swagger spec exists to derive securitySchemes from (the\n  open-source rakam-api Java server generated Swagger at runtime; api.rakam.io is\n  defunct). This profile is searched from the Rakam Data Platform docs.\nsummary:\n  types: [saml, oauth2, apiKey]\n  oauth2_flows: [authorizationCode]\n  sso: true\nschemes:\n  - name: SAML SSO\n    type: saml\n    description: SAML 2.0 single sign-on for platform access (Enterprise plan).\n    docs: https://docs.rakam.io/docs/saml-authentication\n  - name: Google Workspace OAuth2\n    type: oauth2\n    flow: authorizationCode\n    description: GSuite / Google Workspace OAuth2 authentication for platform login.\n    docs: https://docs.rakam.io/docs/google-oauth2-authentication\n  - name: API key (event collection)\n    type: apiKey\n    description:\
  \ >-\n      The open-source rakam-api event-collection server authenticates ingest with\n      project write/master API keys sent by the client SDKs.\n    source: https://github.com/rakam-io/rakam-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rakam/refs/heads/main/authentication/rakam-authentication.yml
summary_line: saml/oauth2/apiKey · 3 schemes
tags:
- Company
- Analytics
- Product Analytics
- Data Warehouse
- Business Intelligence
- Event Tracking
- dbt
- Embedded Analytics
- Semantic Layer
- Open Source
---
