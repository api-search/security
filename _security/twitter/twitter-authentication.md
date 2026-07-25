---
api_key_in: []
api_specs:
- filename: x-ads-api-postman-collection.json
  format: json
  label: X Ads API
  slug: x-ads-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/postman/x-ads-api-postman-collection.json
- filename: twitter-account-activity-api-openapi.yml
  format: yaml
  label: X (Twitter) Account Activity API
  slug: twitter-account-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-account-activity-api-openapi.yml
- filename: twitter-activity-api-openapi.yml
  format: yaml
  label: X (Twitter) Activity API
  slug: twitter-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-activity-api-openapi.yml
- filename: twitter-bookmarks-api-openapi.yml
  format: yaml
  label: X (Twitter) Bookmarks API
  slug: twitter-bookmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-bookmarks-api-openapi.yml
- filename: twitter-chat-api-openapi.yml
  format: yaml
  label: X (Twitter) Chat API
  slug: twitter-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-chat-api-openapi.yml
- filename: twitter-communities-api-openapi.yml
  format: yaml
  label: X (Twitter) Communities API
  slug: twitter-communities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-communities-api-openapi.yml
- filename: twitter-community-notes-api-openapi.yml
  format: yaml
  label: X (Twitter) Community Notes API
  slug: twitter-community-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-community-notes-api-openapi.yml
- filename: twitter-compliance-api-openapi.yml
  format: yaml
  label: X (Twitter) Compliance API
  slug: twitter-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-compliance-api-openapi.yml
- filename: twitter-connections-api-openapi.yml
  format: yaml
  label: X (Twitter) Connections API
  slug: twitter-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-connections-api-openapi.yml
- filename: twitter-direct-messages-api-openapi.yml
  format: yaml
  label: X (Twitter) Direct Messages API
  slug: twitter-direct-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-direct-messages-api-openapi.yml
- filename: twitter-general-api-openapi.yml
  format: yaml
  label: X (Twitter) General API
  slug: twitter-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-general-api-openapi.yml
- filename: twitter-likes-api-openapi.yml
  format: yaml
  label: X (Twitter) Likes API
  slug: twitter-likes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-likes-api-openapi.yml
- filename: twitter-lists-api-openapi.yml
  format: yaml
  label: X (Twitter) Lists API
  slug: twitter-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-lists-api-openapi.yml
- filename: twitter-media-api-openapi.yml
  format: yaml
  label: X (Twitter) Media API
  slug: twitter-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-media-api-openapi.yml
- filename: twitter-news-api-openapi.yml
  format: yaml
  label: X (Twitter) News API
  slug: twitter-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-news-api-openapi.yml
- filename: twitter-spaces-api-openapi.yml
  format: yaml
  label: X (Twitter) Spaces API
  slug: twitter-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-spaces-api-openapi.yml
- filename: twitter-stream-api-openapi.yml
  format: yaml
  label: X (Twitter) Stream API
  slug: twitter-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-stream-api-openapi.yml
- filename: twitter-trends-api-openapi.yml
  format: yaml
  label: X (Twitter) Trends API
  slug: twitter-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-trends-api-openapi.yml
- filename: twitter-tweets-api-openapi.yml
  format: yaml
  label: X (Twitter) Tweets API
  slug: twitter-tweets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-tweets-api-openapi.yml
- filename: twitter-usage-api-openapi.yml
  format: yaml
  label: X (Twitter) Usage API
  slug: twitter-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-usage-api-openapi.yml
- filename: twitter-users-api-openapi.yml
  format: yaml
  label: X (Twitter) Users API
  slug: twitter-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-users-api-openapi.yml
- filename: twitter-webhooks-api-openapi.yml
  format: yaml
  label: X (Twitter) Webhooks API
  slug: twitter-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/openapi/twitter-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Twitter Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: X (Twitter) secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: X (Twitter)
provider_slug: twitter
scheme_count: 3
schemes:
- name: BearerToken
  scheme: bearer
  sources:
  - openapi/x-api-openapi.json
  type: http
- flows:
  - authorizationUrl: https://api.x.com/2/oauth2/authorize
    flow: authorizationCode
    scopes: 21
    tokenUrl: https://api.x.com/2/oauth2/token
  name: OAuth2UserToken
  sources:
  - openapi/x-api-openapi.json
  type: oauth2
- name: UserToken
  scheme: OAuth
  sources:
  - openapi/x-api-openapi.json
  type: http
slug: twitter-authentication
source_filename: twitter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/x-api-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/x-api-openapi.json\n- name: OAuth2UserToken\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.x.com/2/oauth2/authorize\n    tokenUrl: https://api.x.com/2/oauth2/token\n    scopes: 21\n  sources:\n  - openapi/x-api-openapi.json\n- name: UserToken\n  type: http\n  scheme: OAuth\n  sources:\n  - openapi/x-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/authentication/twitter-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
---
