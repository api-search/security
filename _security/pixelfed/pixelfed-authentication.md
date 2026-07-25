---
api_key_in: []
api_specs:
- filename: pixelfed-accounts-api-openapi.yml
  format: yaml
  label: Pixelfed Accounts API
  slug: pixelfed-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-accounts-api-openapi.yml
- filename: pixelfed-blocks-and-mutes-api-openapi.yml
  format: yaml
  label: Pixelfed Blocks and Mutes API
  slug: pixelfed-blocks-and-mutes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-blocks-and-mutes-api-openapi.yml
- filename: pixelfed-bookmarks-api-openapi.yml
  format: yaml
  label: Pixelfed Bookmarks API
  slug: pixelfed-bookmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-bookmarks-api-openapi.yml
- filename: pixelfed-collections-api-openapi.yml
  format: yaml
  label: Pixelfed Collections API
  slug: pixelfed-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-collections-api-openapi.yml
- filename: pixelfed-direct-messages-api-openapi.yml
  format: yaml
  label: Pixelfed Direct Messages API
  slug: pixelfed-direct-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-direct-messages-api-openapi.yml
- filename: pixelfed-discovery-api-openapi.yml
  format: yaml
  label: Pixelfed Discovery API
  slug: pixelfed-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-discovery-api-openapi.yml
- filename: pixelfed-favourites-api-openapi.yml
  format: yaml
  label: Pixelfed Favourites API
  slug: pixelfed-favourites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-favourites-api-openapi.yml
- filename: pixelfed-follow-requests-api-openapi.yml
  format: yaml
  label: Pixelfed Follow Requests API
  slug: pixelfed-follow-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-follow-requests-api-openapi.yml
- filename: pixelfed-instance-api-openapi.yml
  format: yaml
  label: Pixelfed Instance API
  slug: pixelfed-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-instance-api-openapi.yml
- filename: pixelfed-lists-api-openapi.yml
  format: yaml
  label: Pixelfed Lists API
  slug: pixelfed-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-lists-api-openapi.yml
- filename: pixelfed-media-api-openapi.yml
  format: yaml
  label: Pixelfed Media API
  slug: pixelfed-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-media-api-openapi.yml
- filename: pixelfed-notifications-api-openapi.yml
  format: yaml
  label: Pixelfed Notifications API
  slug: pixelfed-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-notifications-api-openapi.yml
- filename: pixelfed-push-notifications-api-openapi.yml
  format: yaml
  label: Pixelfed Push Notifications API
  slug: pixelfed-push-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-push-notifications-api-openapi.yml
- filename: pixelfed-search-api-openapi.yml
  format: yaml
  label: Pixelfed Search API
  slug: pixelfed-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-search-api-openapi.yml
- filename: pixelfed-statuses-api-openapi.yml
  format: yaml
  label: Pixelfed Statuses API
  slug: pixelfed-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-statuses-api-openapi.yml
- filename: pixelfed-stories-api-openapi.yml
  format: yaml
  label: Pixelfed Stories API
  slug: pixelfed-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-stories-api-openapi.yml
- filename: pixelfed-timelines-api-openapi.yml
  format: yaml
  label: Pixelfed Timelines API
  slug: pixelfed-timelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/openapi/pixelfed-timelines-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Pixelfed Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Pixelfed secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Pixelfed
provider_slug: pixelfed
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://{instance}/oauth/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://{instance}/oauth/token
  name: OAuth2
  sources:
  - openapi/openapi.yml
  type: oauth2
- bearerFormat: OAuth2
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: pixelfed-authentication
source_filename: pixelfed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{instance}/oauth/authorize\n    tokenUrl: https://{instance}/oauth/token\n    scopes: 4\n  sources:\n  - openapi/openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: OAuth2\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixelfed/refs/heads/main/authentication/pixelfed-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Fediverse
- ActivityPub
- Photo Sharing
- Social Media
- Open Source
- Decentralized
- Mastodon Compatible
- Federation
---
