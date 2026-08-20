---
api_key_in:
- header
api_specs:
- filename: devto-agent-sessions-api-openapi.yml
  format: yaml
  label: DEV Community agent_sessions API
  slug: devto-agent-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-agent-sessions-api-openapi.yml
- filename: devto-articles-api-openapi.yml
  format: yaml
  label: DEV Community articles API
  slug: devto-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-articles-api-openapi.yml
- filename: devto-billboards-api-openapi.yml
  format: yaml
  label: DEV Community billboards API
  slug: devto-billboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-billboards-api-openapi.yml
- filename: devto-comments-api-openapi.yml
  format: yaml
  label: DEV Community comments API
  slug: devto-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-comments-api-openapi.yml
- filename: devto-display-ads-api-openapi.yml
  format: yaml
  label: DEV Community display ads API
  slug: devto-display-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-display-ads-api-openapi.yml
- filename: devto-followed-tags-api-openapi.yml
  format: yaml
  label: DEV Community followed_tags API
  slug: devto-followed-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-followed-tags-api-openapi.yml
- filename: devto-followers-api-openapi.yml
  format: yaml
  label: DEV Community followers API
  slug: devto-followers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-followers-api-openapi.yml
- filename: devto-organizations-api-openapi.yml
  format: yaml
  label: DEV Community organizations API
  slug: devto-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-organizations-api-openapi.yml
- filename: devto-pages-api-openapi.yml
  format: yaml
  label: DEV Community pages API
  slug: devto-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-pages-api-openapi.yml
- filename: devto-podcast-episodes-api-openapi.yml
  format: yaml
  label: DEV Community podcast_episodes API
  slug: devto-podcast-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-podcast-episodes-api-openapi.yml
- filename: devto-profile-images-api-openapi.yml
  format: yaml
  label: DEV Community profile images API
  slug: devto-profile-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-profile-images-api-openapi.yml
- filename: devto-reactions-api-openapi.yml
  format: yaml
  label: DEV Community reactions API
  slug: devto-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-reactions-api-openapi.yml
- filename: devto-readinglist-api-openapi.yml
  format: yaml
  label: DEV Community readinglist API
  slug: devto-readinglist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-readinglist-api-openapi.yml
- filename: devto-segments-api-openapi.yml
  format: yaml
  label: DEV Community segments API
  slug: devto-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-segments-api-openapi.yml
- filename: devto-surveys-api-openapi.yml
  format: yaml
  label: DEV Community surveys API
  slug: devto-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-surveys-api-openapi.yml
- filename: devto-tags-api-openapi.yml
  format: yaml
  label: DEV Community tags API
  slug: devto-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-tags-api-openapi.yml
- filename: devto-trends-api-openapi.yml
  format: yaml
  label: DEV Community trends API
  slug: devto-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-trends-api-openapi.yml
- filename: devto-users-api-openapi.yml
  format: yaml
  label: DEV Community users API
  slug: devto-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-users-api-openapi.yml
- filename: devto-videos-api-openapi.yml
  format: yaml
  label: DEV Community videos API
  slug: devto-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/openapi/devto-videos-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Devto Authentication
name_suffix: Authentication
oauth_flows: []
overview: DEV Community secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DEV Community
provider_slug: devto
scheme_count: 1
schemes:
- description: "API Key authentication.\n\nAuthentication for some endpoints, like write operations on the\nArticles API require a DEV API key.\n\nAll authenticated endpoints are CORS disabled, the API key is intended for non-browser scripts.\n\n### Getting an API key\n\nTo obtain one, please follow these steps:\n\n  - visit https://dev.to/settings/extensions\n  - in the \"DEV API Keys\" section create a new key by adding a\n  "
  in: header
  name: api-key
  parameter: api-key
  sources:
  - openapi/openapi.json
  - openapi/openapi.yaml
  type: apiKey
slug: devto-authentication
source_filename: devto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json, openapi/openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: \"API Key authentication.\\n\\nAuthentication for some endpoints, like write operations\\\n    \\ on the\\nArticles API require a DEV API key.\\n\\nAll authenticated endpoints are CORS disabled,\\\n    \\ the API key is intended for non-browser scripts.\\n\\n### Getting an API key\\n\\nTo obtain\\\n    \\ one, please follow these steps:\\n\\n  - visit https://dev.to/settings/extensions\\n  - in\\\n    \\ the \\\"DEV API Keys\\\" section create a new key by adding a\\n  \"\n  sources:\n  - openapi/openapi.json\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devto/refs/heads/main/authentication/devto-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Developer Community
- Articles
- Blogging
- Social
- Content
- Open-Source
---
