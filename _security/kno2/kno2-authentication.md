---
api_key_in: []
api_specs:
- filename: kno2-openapi.yml
  format: yaml
  label: Kno2 Messaging API
  slug: kno2-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-openapi.yml
- filename: kno2-openapi.yml
  format: yaml
  label: Kno2 Intake and Retrieval API
  slug: kno2-intake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-openapi.yml
- filename: kno2-openapi.yml
  format: yaml
  label: Kno2 Directory API
  slug: kno2-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/openapi/kno2-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kno2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kno2 secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kno2
provider_slug: kno2
scheme_count: 3
schemes:
- description: OAuth2 client-credentials flow. Authenticate to POST /api/token with HTTP Basic using base64(client_id:client_secret) and grant_type=client_credentials to receive a Bearer access token. A grant_type=refresh_token flow is also supported. Credentials (client id, client secret, app id) are provisioned by Kno2, and your public IP must be allowlisted by a Kno2 admin.
  flow: clientCredentials
  name: oauth2ClientCredentials
  sources:
  - https://github.com/Kno2/Kno2.ApiTestClient
  tokenUrl: https://{subscription}.kno2fy.com/api/token
  type: oauth2
- description: 'All Communication API requests carry the OAuth2 access token as `Authorization: Bearer <token>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kno2-openapi.yml
  type: http
- description: HTTP Basic base64(client_id:client_secret), used only against /api/token to obtain a Bearer token.
  name: basicAuth
  scheme: basic
  sources:
  - https://github.com/Kno2/Kno2.ApiTestClient
  type: http
slug: kno2-authentication
source_filename: kno2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/kno2-openapi.yml\nnotes: >-\n  Confirmed from Kno2's official Kno2.ApiTestClient. The token endpoint,\n  client-credentials grant, HTTP Basic client authentication, and Bearer usage\n  are grounded in the reference client's ApiHelper.cs and app.config; full\n  field-level details are provisioned per partner via the login-walled developer\n  portal at developer.kno2.com.\nsummary:\n  types:\n  - oauth2\n  - http\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://{subscription}.kno2fy.com/api/token\n  description: >-\n    OAuth2 client-credentials flow. Authenticate to POST /api/token with HTTP\n    Basic using base64(client_id:client_secret) and grant_type=client_credentials\n    to receive a Bearer access token. A grant_type=refresh_token flow is also\n    supported. Credentials (client id, client secret, app id) are provisioned by\n    Kno2, and your public IP\
  \ must be allowlisted by a Kno2 admin.\n  sources:\n  - https://github.com/Kno2/Kno2.ApiTestClient\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    All Communication API requests carry the OAuth2 access token as\n    `Authorization: Bearer <token>`.\n  sources:\n  - openapi/kno2-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic base64(client_id:client_secret), used only against /api/token to\n    obtain a Bearer token.\n  sources:\n  - https://github.com/Kno2/Kno2.ApiTestClient\nnotesSecurity: >-\n  Kno2 requires TLS 1.2 or higher for all integrations and enforces an IP\n  allowlist per subscription. Exchange involves protected health information\n  (PHI) and is governed by HIPAA and Kno2's network/QHIN participation\n  agreements.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kno2/refs/heads/main/authentication/kno2-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Healthcare Interoperability
- Clinical Records
- Health Information Exchange
- Direct Secure Messaging
- FHIR
- Clinical Documents
- Patient Records
- Healthcare
- HIE
- Care Coordination
- QHIN
- TEFCA
- Carequality
---
