---
api_key_in: []
api_specs:
- filename: sequel-analytics-api-openapi.yml
  format: yaml
  label: Sequel Analytics API
  slug: sequel-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-analytics-api-openapi.yml
- filename: sequel-client-api-openapi.yml
  format: yaml
  label: Sequel Client API
  slug: sequel-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-client-api-openapi.yml
- filename: sequel-company-api-openapi.yml
  format: yaml
  label: Sequel company API
  slug: sequel-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-api-openapi.yml
- filename: sequel-company-theme-api-openapi.yml
  format: yaml
  label: Sequel company theme API
  slug: sequel-company-theme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-theme-api-openapi.yml
- filename: sequel-company-theme-fonts-api-openapi.yml
  format: yaml
  label: Sequel company theme fonts API
  slug: sequel-company-theme-fonts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-theme-fonts-api-openapi.yml
- filename: sequel-company-theme-overrides-api-openapi.yml
  format: yaml
  label: Sequel company theme overrides API
  slug: sequel-company-theme-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-company-theme-overrides-api-openapi.yml
- filename: sequel-event-api-openapi.yml
  format: yaml
  label: Sequel event API
  slug: sequel-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-event-api-openapi.yml
- filename: sequel-event-theme-api-openapi.yml
  format: yaml
  label: Sequel event theme API
  slug: sequel-event-theme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-event-theme-api-openapi.yml
- filename: sequel-event-theme-overrides-api-openapi.yml
  format: yaml
  label: Sequel event theme overrides API
  slug: sequel-event-theme-overrides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-event-theme-overrides-api-openapi.yml
- filename: sequel-media-api-openapi.yml
  format: yaml
  label: Sequel Media API
  slug: sequel-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-media-api-openapi.yml
- filename: sequel-networking-api-openapi.yml
  format: yaml
  label: Sequel networking API
  slug: sequel-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-networking-api-openapi.yml
- filename: sequel-platform-api-openapi.yml
  format: yaml
  label: Sequel platform API
  slug: sequel-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-platform-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sequel Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Sequel secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Sequel
provider_slug: sequel
scheme_count: 2
schemes:
- audience: https://www.introvoke.com/api
  credentials: client_id + client_secret from the Sequel Admin Dashboard > Integrations > APIs
  flow: clientCredentials
  grant_type: client_credentials
  name: oauth2ClientCredentials
  request_body: "{\n  \"client_id\": \"<your_client_id>\",\n  \"client_secret\": \"<your_client_secret>\",\n  \"audience\": \"https://www.introvoke.com/api\",\n  \"grant_type\": \"client_credentials\"\n}"
  response: returns access_token and token_type "Bearer"
  source: searched (https://docs.introvoke.com/docs)
  token_url: https://api.introvoke.com/api/oauth/token
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sequel-openapi-original.yml
  type: http
  usage: 'Authorization: Bearer <access_token>'
slug: sequel-authentication
source_filename: sequel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sequel-openapi-original.yml\ndocs: https://docs.introvoke.com/docs\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  bearer_format: JWT\n  notes: >-\n    The Sequel (Introvoke) API is protected with an OAuth 2.0 client-credentials\n    flow. Exchange a client_id/client_secret for a JWT access token, then send it\n    as an HTTP bearer token on every API call. End-user / admin login to the Sequel\n    dashboard is a separate Auth0 OpenID Connect authorization-code flow.\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.introvoke.com/api/oauth/token\n  audience: https://www.introvoke.com/api\n  grant_type: client_credentials\n  credentials: client_id + client_secret from the Sequel Admin Dashboard > Integrations > APIs\n  request_body: |-\n    {\n      \"client_id\": \"<your_client_id>\",\n      \"client_secret\": \"<your_client_secret>\"\
  ,\n      \"audience\": \"https://www.introvoke.com/api\",\n      \"grant_type\": \"client_credentials\"\n    }\n  response: returns access_token and token_type \"Bearer\"\n  source: searched (https://docs.introvoke.com/docs)\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  usage: 'Authorization: Bearer <access_token>'\n  sources:\n  - openapi/sequel-openapi-original.yml\nend_user_login:\n  provider: Auth0\n  type: openIdConnect\n  issuer: https://login.introvoke.com\n  authorization_endpoint: https://login.introvoke.com/authorize\n  token_endpoint: https://login.introvoke.com/oauth/token\n  flows:\n  - authorization_code\n  - refresh_token\n  scopes_supported:\n  - openid\n  - profile\n  - email\n  - offline_access\n  source: well-known/sequel-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/authentication/sequel-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Webinars
- Virtual Events
- Live Streaming
- Video
- Networking
- Marketing
- Events
- Webhooks
---
