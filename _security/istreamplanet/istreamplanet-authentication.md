---
anonymous_access: false
api_key_in: []
api_specs:
- filename: istreamplanet-audit-operations-for-organization-api-openapi.yml
  format: yaml
  label: iStreamPlanet Audit Operations for Organization API
  slug: istreamplanet-audit-operations-for-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-audit-operations-for-organization-api-openapi.yml
- filename: istreamplanet-available-sources-api-openapi.yml
  format: yaml
  label: iStreamPlanet Available Sources API
  slug: istreamplanet-available-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-available-sources-api-openapi.yml
- filename: istreamplanet-channel-operations-for-organization-api-openapi.yml
  format: yaml
  label: iStreamPlanet Channel Operations for Organization API
  slug: istreamplanet-channel-operations-for-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-channel-operations-for-organization-api-openapi.yml
- filename: istreamplanet-channels-api-openapi.yml
  format: yaml
  label: iStreamPlanet Channels API
  slug: istreamplanet-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-channels-api-openapi.yml
- filename: istreamplanet-channels-for-organization-api-openapi.yml
  format: yaml
  label: iStreamPlanet Channels for Organization API
  slug: istreamplanet-channels-for-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-channels-for-organization-api-openapi.yml
- filename: istreamplanet-deprecated-live2vod-api-openapi.yml
  format: yaml
  label: iStreamPlanet Deprecated Live2VOD API
  slug: istreamplanet-deprecated-live2vod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-deprecated-live2vod-api-openapi.yml
- filename: istreamplanet-live2vod-for-organization-api-openapi.yml
  format: yaml
  label: iStreamPlanet Live2VOD for Organization API
  slug: istreamplanet-live2vod-for-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-live2vod-for-organization-api-openapi.yml
- filename: istreamplanet-organizations-api-openapi.yml
  format: yaml
  label: iStreamPlanet Organizations API
  slug: istreamplanet-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-organizations-api-openapi.yml
- filename: istreamplanet-source-previews-api-openapi.yml
  format: yaml
  label: iStreamPlanet Source Previews API
  slug: istreamplanet-source-previews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-source-previews-api-openapi.yml
- filename: istreamplanet-transcoder-telemetry-api-openapi.yml
  format: yaml
  label: iStreamPlanet Transcoder Telemetry API
  slug: istreamplanet-transcoder-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/openapi/istreamplanet-transcoder-telemetry-api-openapi.yml
auth_types:
- oauth2
description: Auth is handled via the WBD Okta offering using RFC 7519 JSON Web Tokens (JWT). Clients first make a request to the application's WBD Okta endpoint to get a token, and then provide that token in an `Authorization` header with each request to the API. Tokens are short lived and a new token must be fetched when the token expires. WBD Okta supports RFC 6749 OAuth 2.0, both the Authorization Code (with PKCE) and Client Credential grant flows.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Istreamplanet Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: iStreamPlanet secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: iStreamPlanet
provider_slug: istreamplanet
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://sso.wbd.com/oauth2/aus125bl6q770za4g0x8/v1/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://sso.wbd.com/oauth2/aus125bl6q770za4g0x8/v1/token
  name: authcode
  sources:
  - openapi/istreamplanet-aventus-channels-openapi.yml
  type: oauth2
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://sso.wbd.com/oauth2/aus125bl6q770za4g0x8/v1/token
  name: m2m
  sources:
  - openapi/istreamplanet-aventus-channels-openapi.yml
  type: oauth2
slug: istreamplanet-authentication
source_filename: istreamplanet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: https://api.istreamplanet.com/docs\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: authcode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sso.wbd.com/oauth2/aus125bl6q770za4g0x8/v1/authorize\n    tokenUrl: https://sso.wbd.com/oauth2/aus125bl6q770za4g0x8/v1/token\n    scopes: 0\n  sources:\n  - openapi/istreamplanet-aventus-channels-openapi.yml\n- name: m2m\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sso.wbd.com/oauth2/aus125bl6q770za4g0x8/v1/token\n    scopes: 0\n  sources:\n  - openapi/istreamplanet-aventus-channels-openapi.yml\ndocs: https://api.istreamplanet.com/docs\nderived_from: openapi/istreamplanet-aventus-channels-openapi.yml\ndescription: Auth is handled via the WBD Okta offering using RFC 7519 JSON Web Tokens (JWT). Clients first make a request\n  to the application's WBD Okta\
  \ endpoint to get a token, and then provide that token in an `Authorization` header with each\n  request to the API. Tokens are short lived and a new token must be fetched when the token expires. WBD Okta supports RFC\n  6749 OAuth 2.0, both the Authorization Code (with PKCE) and Client Credential grant flows.\ntoken_format: JWT (RFC 7519)\nidentity_provider: WBD Okta (sso.wbd.com)\npkce: true\ncredentials:\n  source: https://istreamlabs.github.io/docs/guide/\n  text: OAuth2 client ID for calling the API (optional) OAuth2 client secret for machine-to-machine use-cases\n  provisioning: contact iStreamPlanet to set up a new organization, or ask your administrator to create a user account in\n    the Portal UI\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/istreamplanet/refs/heads/main/authentication/istreamplanet-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Video Streaming
- Live Streaming
- Media
- Cloud Video
- Spectral
- API Governance
---
