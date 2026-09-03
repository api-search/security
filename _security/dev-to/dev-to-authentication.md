---
api_key_in:
- header
api_specs:
- filename: dev-to-webhooks-asyncapi.yml
  format: yaml
  label: Dev.to Webhooks API
  slug: webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/asyncapi/dev-to-webhooks-asyncapi.yml
- filename: dev-to-articles-api-openapi.yml
  format: yaml
  label: dev-to Articles API
  slug: dev-to-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-articles-api-openapi.yml
- filename: dev-to-comments-api-openapi.yml
  format: yaml
  label: dev-to Comments API
  slug: dev-to-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-comments-api-openapi.yml
- filename: dev-to-displayads-api-openapi.yml
  format: yaml
  label: dev-to DisplayAds API
  slug: dev-to-displayads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-displayads-api-openapi.yml
- filename: dev-to-followedtags-api-openapi.yml
  format: yaml
  label: dev-to FollowedTags API
  slug: dev-to-followedtags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-followedtags-api-openapi.yml
- filename: dev-to-followers-api-openapi.yml
  format: yaml
  label: dev-to Followers API
  slug: dev-to-followers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-followers-api-openapi.yml
- filename: dev-to-organizations-api-openapi.yml
  format: yaml
  label: dev-to Organizations API
  slug: dev-to-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-organizations-api-openapi.yml
- filename: dev-to-pages-api-openapi.yml
  format: yaml
  label: dev-to Pages API
  slug: dev-to-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-pages-api-openapi.yml
- filename: dev-to-podcastepisodes-api-openapi.yml
  format: yaml
  label: dev-to PodcastEpisodes API
  slug: dev-to-podcastepisodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-podcastepisodes-api-openapi.yml
- filename: dev-to-profileimages-api-openapi.yml
  format: yaml
  label: dev-to ProfileImages API
  slug: dev-to-profileimages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-profileimages-api-openapi.yml
- filename: dev-to-reactions-api-openapi.yml
  format: yaml
  label: dev-to Reactions API
  slug: dev-to-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-reactions-api-openapi.yml
- filename: dev-to-readinglist-api-openapi.yml
  format: yaml
  label: dev-to ReadingList API
  slug: dev-to-readinglist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-readinglist-api-openapi.yml
- filename: dev-to-tags-api-openapi.yml
  format: yaml
  label: dev-to Tags API
  slug: dev-to-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-tags-api-openapi.yml
- filename: dev-to-users-api-openapi.yml
  format: yaml
  label: dev-to Users API
  slug: dev-to-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-users-api-openapi.yml
- filename: dev-to-webhooks-api-openapi.yml
  format: yaml
  label: dev-to Webhooks API
  slug: dev-to-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dev To Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dev To secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dev To
provider_slug: dev-to
scheme_count: 1
schemes:
- description: API key obtained from the DEV.to settings page. Pass in the api-key header for authenticated requests.
  in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/dev-to-forem-api-openapi.yml
  type: apiKey
slug: dev-to-authentication
source_filename: dev-to-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dev-to-forem-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: API key obtained from the DEV.to settings page. Pass in the api-key header for\n    authenticated requests.\n  sources:\n  - openapi/dev-to-forem-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/authentication/dev-to-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
