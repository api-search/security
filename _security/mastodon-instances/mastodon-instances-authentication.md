---
api_key_in: []
api_specs:
- filename: mastodon-instances-instances-api-openapi.yml
  format: yaml
  label: Mastodon Instances Instances API
  slug: mastodon-instances-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastodon-instances/refs/heads/main/openapi/mastodon-instances-instances-api-openapi.yml
- filename: mastodon-instances-versions-api-openapi.yml
  format: yaml
  label: Mastodon Instances Versions API
  slug: mastodon-instances-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mastodon-instances/refs/heads/main/openapi/mastodon-instances-versions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mastodon Instances Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mastodon Instances secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mastodon Instances
provider_slug: mastodon-instances
scheme_count: 1
schemes:
- description: 'API token obtained from https://instances.social/api/token,

    passed as `Authorization: Bearer {token}`.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/mastodon-instances-openapi.yml
  type: http
slug: mastodon-instances-authentication
source_filename: mastodon-instances-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mastodon-instances-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    API token obtained from https://instances.social/api/token,\n    passed as `Authorization: Bearer {token}`.\n  sources:\n  - openapi/mastodon-instances-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mastodon-instances/refs/heads/main/authentication/mastodon-instances-authentication.yml
summary_line: http · 1 scheme
tags:
- Fediverse
- Mastodon
- Search
- Social
---
