---
api_key_in:
- header
api_specs:
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Assets API
  slug: mediavalet-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Categories API
  slug: mediavalet-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Attributes API
  slug: mediavalet-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Keywords API
  slug: mediavalet-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Uploads API
  slug: mediavalet-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
- filename: mediavalet-openapi.yml
  format: yaml
  label: MediaValet Users API
  slug: mediavalet-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/openapi/mediavalet-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Mediavalet Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MediaValet secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MediaValet
provider_slug: mediavalet
scheme_count: 2
schemes:
- description: OAuth 2.0 / OpenID Connect. Obtain an access token from https://login.mediavalet.com/connect/token using the authorization code flow (interactive apps) or password / client-credential grants, with scopes openid api offline_access. Send the token as a Bearer Authorization header.
  flows:
  - authorizationUrl: https://login.mediavalet.com/connect/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://login.mediavalet.com/connect/token
  name: oauth2
  sources:
  - openapi/mediavalet-openapi.yml
  type: oauth2
- description: Per-account API subscription key issued through the MediaValet Developer Portal.
  in: header
  name: subscriptionKey
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/mediavalet-openapi.yml
  type: apiKey
slug: mediavalet-authentication
source_filename: mediavalet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mediavalet-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.mediavalet.com/connect/authorize\n    tokenUrl: https://login.mediavalet.com/connect/token\n    scopes: 3\n  description: OAuth 2.0 / OpenID Connect. Obtain an access token from https://login.mediavalet.com/connect/token\n    using the authorization code flow (interactive apps) or password / client-credential grants,\n    with scopes openid api offline_access. Send the token as a Bearer Authorization header.\n  sources:\n  - openapi/mediavalet-openapi.yml\n- name: subscriptionKey\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: Per-account API subscription key issued through the MediaValet Developer Portal.\n  sources:\n  - openapi/mediavalet-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mediavalet/refs/heads/main/authentication/mediavalet-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Digital Asset Management
- DAM
- Media
- Assets
- Content
- Marketing
- Cloud Storage
---
