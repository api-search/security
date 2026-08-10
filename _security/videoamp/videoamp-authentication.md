---
api_key_in: []
api_specs:
- filename: videoamp-admeasurements-api-openapi.yml
  format: yaml
  label: VideoAmp Ad Measurements API
  slug: videoamp-admeasurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-admeasurements-api-openapi.yml
- filename: videoamp-audiences-api-openapi.yml
  format: yaml
  label: VideoAmp Audiences API
  slug: videoamp-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-audiences-api-openapi.yml
- filename: videoamp-campaigns-api-openapi.yml
  format: yaml
  label: VideoAmp Campaigns API
  slug: videoamp-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-campaigns-api-openapi.yml
- filename: videoamp-consents-api-openapi.yml
  format: yaml
  label: VideoAmp Consents API
  slug: videoamp-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-consents-api-openapi.yml
- filename: videoamp-content-api-openapi.yml
  format: yaml
  label: VideoAmp Content API
  slug: videoamp-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-content-api-openapi.yml
- filename: videoamp-currency-of-record-api-openapi.yml
  format: yaml
  label: VideoAmp Currency Of Record API
  slug: videoamp-currency-of-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-currency-of-record-api-openapi.yml
- filename: videoamp-datastreams-api-openapi.yml
  format: yaml
  label: VideoAmp Data Streams API
  slug: videoamp-datastreams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-datastreams-api-openapi.yml
- filename: videoamp-datastreamtypes-api-openapi.yml
  format: yaml
  label: VideoAmp Data Stream Types API
  slug: videoamp-datastreamtypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-datastreamtypes-api-openapi.yml
- filename: videoamp-inventories-api-openapi.yml
  format: yaml
  label: VideoAmp Inventories API
  slug: videoamp-inventories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-inventories-api-openapi.yml
- filename: videoamp-library-api-openapi.yml
  format: yaml
  label: VideoAmp Library API
  slug: videoamp-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-library-api-openapi.yml
- filename: videoamp-me-api-openapi.yml
  format: yaml
  label: VideoAmp Me API
  slug: videoamp-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-me-api-openapi.yml
- filename: videoamp-plans-api-openapi.yml
  format: yaml
  label: VideoAmp Plans API
  slug: videoamp-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-plans-api-openapi.yml
- filename: videoamp-reports-api-openapi.yml
  format: yaml
  label: VideoAmp Reports API
  slug: videoamp-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-reports-api-openapi.yml
- filename: videoamp-shares-api-openapi.yml
  format: yaml
  label: VideoAmp Shares API
  slug: videoamp-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/openapi/videoamp-shares-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Videoamp Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceAuthorization
overview: VideoAmp secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and deviceAuthorization flow(s).
provider_name: VideoAmp
provider_slug: videoamp
scheme_count: 1
schemes:
- description: OAuth 2.0 / OIDC via VideoAmp's Auth0 tenant at https://login.videoamp.com. Verified from https://login.videoamp.com/.well-known/openid-configuration (HTTP 200) and https://api.videoamp.dev/.well-known/oauth-protected-resource/v1/mcp (HTTP 200, RFC 9728). Bearer tokens are presented in the Authorization header.
  flows:
  - authorizationUrl: https://login.videoamp.com/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://login.videoamp.com/oauth/token
  - flow: deviceAuthorization
    scopes: 4
    tokenUrl: https://login.videoamp.com/oauth/token
  name: videoampOAuth
  sources:
  - openapi/videoamp-public-api-openapi.yml
  type: oauth2
slug: videoamp-authentication
source_filename: videoamp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/videoamp-public-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - deviceAuthorization\nschemes:\n- name: videoampOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.videoamp.com/authorize\n    tokenUrl: https://login.videoamp.com/oauth/token\n    scopes: 4\n  - flow: deviceAuthorization\n    tokenUrl: https://login.videoamp.com/oauth/token\n    scopes: 4\n  description: OAuth 2.0 / OIDC via VideoAmp's Auth0 tenant at https://login.videoamp.com. Verified\n    from https://login.videoamp.com/.well-known/openid-configuration (HTTP 200) and https://api.videoamp.dev/.well-known/oauth-protected-resource/v1/mcp\n    (HTTP 200, RFC 9728). Bearer tokens are presented in the Authorization header.\n  sources:\n  - openapi/videoamp-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/videoamp/refs/heads/main/authentication/videoamp-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- media-measurement
- advertising
- adtech
- tv-currency
- audience-measurement
- media-planning
- streaming
- attribution
- data-collaboration
- mcp
- agent-native
---
