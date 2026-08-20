---
api_key_in:
- header
- query
api_specs:
- filename: banzai-events-api-openapi.yml
  format: yaml
  label: Banzai Events API
  slug: banzai-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banzai/refs/heads/main/openapi/banzai-events-api-openapi.yml
- filename: banzai-intro-api-openapi.yml
  format: yaml
  label: Banzai Intro API
  slug: banzai-intro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banzai/refs/heads/main/openapi/banzai-intro-api-openapi.yml
- filename: banzai-reports-api-openapi.yml
  format: yaml
  label: Banzai Reports API
  slug: banzai-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/banzai/refs/heads/main/openapi/banzai-reports-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Banzai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Banzai secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Banzai
provider_slug: banzai
scheme_count: 4
schemes:
- description: Account API Key, from Demio Settings > API.
  in: header
  name: ApiKeyHeader
  parameter: Api-Key
  sources:
  - openapi/banzai-demio-openapi.yml
  type: apiKey
- description: Account API Secret, from Demio Settings > API.
  in: header
  name: ApiSecretHeader
  parameter: Api-Secret
  sources:
  - openapi/banzai-demio-openapi.yml
  type: apiKey
- description: Account API Key supplied on the query string.
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/banzai-demio-openapi.yml
  type: apiKey
- description: Account API Secret supplied on the query string.
  in: query
  name: ApiSecretQuery
  parameter: api_secret
  sources:
  - openapi/banzai-demio-openapi.yml
  type: apiKey
slug: banzai-authentication
source_filename: banzai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: openapi/banzai-demio-openapi.yml\ndocs: https://publicdemioapi.docs.apiary.io\ndocs_secondary:\n- https://help.demio.com/en/articles/4544025-api-limitations\nkey_management:\n  console: https://my.demio.com/manage/api-details\n  note: >-\n    API Key and API Secret are issued per Demio account from Settings > API. The same\n    tab reports daily API-call usage against the account quota. Credentials may be\n    sent as Api-Key/Api-Secret headers or as api_key/api_secret query parameters; the\n    header form is the documented default and the only form that keeps the secret out\n    of URLs and logs.\n  sandbox: >-\n    A sandbox key/secret pair exists — GET /ping returns a `sandbox` boolean that is\n    true when sandbox credentials were used. Demio does not publish a self-serve\n    procedure for obtaining sandbox credentials.\naccount_security:\n  two_factor: https://help.demio.com/en/articles/4794494-two-factor-authentication-2fa\n\
  \  saml_sso: https://help.demio.com/en/articles/8912841-saml-single-sign-on-sso\n  saml_note: >-\n    SAML 2.0 single sign-on covers the Demio web application (select plans, configured\n    by the Demio team). It is not an API authorization mechanism — the API remains\n    key/secret only, with no OAuth 2.0 or OpenID Connect surface.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: Account API Key, from Demio Settings > API.\n  sources:\n  - openapi/banzai-demio-openapi.yml\n- name: ApiSecretHeader\n  type: apiKey\n  in: header\n  parameter: Api-Secret\n  description: Account API Secret, from Demio Settings > API.\n  sources:\n  - openapi/banzai-demio-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Account API Key supplied on the query string.\n  sources:\n  - openapi/banzai-demio-openapi.yml\n- name: ApiSecretQuery\n\
  \  type: apiKey\n  in: query\n  parameter: api_secret\n  description: Account API Secret supplied on the query string.\n  sources:\n  - openapi/banzai-demio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/banzai/refs/heads/main/authentication/banzai-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Company
- Marketing
- Marketing Technology
- Event Management
- Webinars
- Video
- Engagement Marketing
- Demand Generation
- Software-as-a-Service
---
