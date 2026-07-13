---
api_key_in: []
api_specs:
- filename: cms-api-swagger.yaml
  format: yaml
  label: Brightcove CMS API
  slug: brightcove-cms-api
  spec_type: OpenAPI
  url: https://apis.support.brightcove.com/cms/references/cms-api-swagger.yaml
- filename: ssai-openapi.yaml
  format: yaml
  label: Brightcove SSAI API
  slug: brightcove-ssai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightcove/refs/heads/main/openapi/ssai-openapi.yaml
- filename: delivery-rules-openapi.yaml
  format: yaml
  label: Brightcove Delivery Rules API
  slug: brightcove-delivery-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightcove/refs/heads/main/openapi/delivery-rules-openapi.yaml
- filename: social-openapi.yaml
  format: yaml
  label: Brightcove Social API
  slug: brightcove-social-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightcove/refs/heads/main/openapi/social-openapi.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Brightcove Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Brightcove secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Brightcove
provider_slug: brightcove
scheme_count: 1
schemes:
- description: Brightcove OAuth API. See the [support documentation](/oauth/index.html) or [Getting Access Tokens](/oauth/code-samples/oauth-api-sample-get-access-token.html) to learn more
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://oauth.brightcove.com/v4/access_token
  name: BC_OAuth2
  sources:
  - openapi/analytics-api-openapi.yaml
  - openapi/audience-openapi.yaml
  - openapi/cms-api-openapi.yaml
  - openapi/delivery-rules-openapi.yaml
  - openapi/dynamic-ingest-openapi.yaml
  - openapi/ingest-profiles-openapi.yaml
  - openapi/player-management-openapi.yaml
  - openapi/social-openapi.yaml
  - openapi/ssai-openapi.yaml
  type: oauth2
slug: brightcove-authentication
source_filename: brightcove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/analytics-api-openapi.yaml, openapi/audience-openapi.yaml, openapi/cms-api-openapi.yaml,\n  openapi/delivery-rules-openapi.yaml, openapi/dynamic-ingest-openapi.yaml, openapi/ingest-profiles-openapi.yaml,\n  openapi/player-management-openapi.yaml, openapi/social-openapi.yaml, openapi/ssai-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: BC_OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://oauth.brightcove.com/v4/access_token\n    scopes: 2\n  description: Brightcove OAuth API. See the [support documentation](/oauth/index.html) or [Getting\n    Access Tokens](/oauth/code-samples/oauth-api-sample-get-access-token.html) to learn more\n  sources:\n  - openapi/analytics-api-openapi.yaml\n  - openapi/audience-openapi.yaml\n  - openapi/cms-api-openapi.yaml\n  - openapi/delivery-rules-openapi.yaml\n  - openapi/dynamic-ingest-openapi.yaml\n\
  \  - openapi/ingest-profiles-openapi.yaml\n  - openapi/player-management-openapi.yaml\n  - openapi/social-openapi.yaml\n  - openapi/ssai-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightcove/refs/heads/main/authentication/brightcove-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Video
- Media
- Streaming
- Live Streaming
- Analytics
- CDN
- OTT
- Player
- Ad Insertion
---
