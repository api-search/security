---
api_key_in: []
api_specs:
- filename: wistia-asyncapi.yml
  format: yaml
  label: Wistia Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/asyncapi/wistia-asyncapi.yml
- filename: wistia-account-api-openapi.yml
  format: yaml
  label: Wistia Account API
  slug: wistia-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-account-api-openapi.yml
- filename: wistia-alloweddomains-api-openapi.yml
  format: yaml
  label: Wistia AllowedDomains API
  slug: wistia-alloweddomains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-alloweddomains-api-openapi.yml
- filename: wistia-captions-api-openapi.yml
  format: yaml
  label: Wistia Captions API
  slug: wistia-captions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-captions-api-openapi.yml
- filename: wistia-channels-api-openapi.yml
  format: yaml
  label: Wistia Channels API
  slug: wistia-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-channels-api-openapi.yml
- filename: wistia-customizations-api-openapi.yml
  format: yaml
  label: Wistia Customizations API
  slug: wistia-customizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-customizations-api-openapi.yml
- filename: wistia-folders-api-openapi.yml
  format: yaml
  label: Wistia Folders API
  slug: wistia-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-folders-api-openapi.yml
- filename: wistia-medias-api-openapi.yml
  format: yaml
  label: Wistia Medias API
  slug: wistia-medias-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-medias-api-openapi.yml
- filename: wistia-tags-api-openapi.yml
  format: yaml
  label: Wistia Tags API
  slug: wistia-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-tags-api-openapi.yml
- filename: wistia-tokens-api-openapi.yml
  format: yaml
  label: Wistia Tokens API
  slug: wistia-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-tokens-api-openapi.yml
- filename: wistia-webinars-api-openapi.yml
  format: yaml
  label: Wistia Webinars API
  slug: wistia-webinars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/openapi/wistia-webinars-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wistia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wistia secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wistia
provider_slug: wistia
scheme_count: 2
schemes:
- description: API access token sent as a Bearer token in the Authorization header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/wistia-openapi.yml
  type: http
- description: HTTP Basic authentication using the API token as the password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/wistia-openapi.yml
  type: http
slug: wistia-authentication
source_filename: wistia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wistia-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API access token sent as a Bearer token in the Authorization header\n  sources:\n  - openapi/wistia-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using the API token as the password\n  sources:\n  - openapi/wistia-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wistia/refs/heads/main/authentication/wistia-authentication.yml
summary_line: http · 2 schemes
tags:
- Video Hosting
- Video Marketing
- Video Analytics
- Lead Generation
- Webinars
- B2B Marketing
---
