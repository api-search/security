---
api_key_in: []
api_specs:
- filename: threads-api-authorization-api-openapi.yml
  format: yaml
  label: Threads Authorization API
  slug: threads-api-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threads-api/refs/heads/main/openapi/threads-api-authorization-api-openapi.yml
- filename: threads-api-post-to-threads-quote-threads-posts-api-openapi.yml
  format: yaml
  label: Threads Post to Threads > Quote Threads Posts API
  slug: threads-api-post-to-threads-quote-threads-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threads-api/refs/heads/main/openapi/threads-api-post-to-threads-quote-threads-posts-api-openapi.yml
- filename: threads-api-post-to-threads-repost-threads-posts-api-openapi.yml
  format: yaml
  label: Threads Post to Threads > Repost Threads Posts API
  slug: threads-api-post-to-threads-repost-threads-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threads-api/refs/heads/main/openapi/threads-api-post-to-threads-repost-threads-posts-api-openapi.yml
- filename: threads-api-read-and-manage-threads-read-and-manage-threads-replies-api-openapi.yml
  format: yaml
  label: Threads Read And Manage Threads > Read and Manage Threads Replies API
  slug: threads-api-read-and-manage-threads-read-and-manage-threads-replies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threads-api/refs/heads/main/openapi/threads-api-read-and-manage-threads-read-and-manage-threads-replies-api-openapi.yml
- filename: threads-api-read-and-manage-threads-read-replies-media-objects-api-openapi.yml
  format: yaml
  label: Threads Read And Manage Threads > Read Replies Media Objects API
  slug: threads-api-read-and-manage-threads-read-replies-media-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threads-api/refs/heads/main/openapi/threads-api-read-and-manage-threads-read-replies-media-objects-api-openapi.yml
- filename: threads-api-read-and-manage-threads-read-threads-insights-api-openapi.yml
  format: yaml
  label: Threads Read And Manage Threads > Read Threads Insights API
  slug: threads-api-read-and-manage-threads-read-threads-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threads-api/refs/heads/main/openapi/threads-api-read-and-manage-threads-read-threads-insights-api-openapi.yml
- filename: threads-api-read-and-manage-threads-retrieve-threads-media-objects-api-openapi.yml
  format: yaml
  label: Threads Read And Manage Threads > Retrieve Threads Media Objects API
  slug: threads-api-read-and-manage-threads-retrieve-threads-media-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threads-api/refs/heads/main/openapi/threads-api-read-and-manage-threads-retrieve-threads-media-objects-api-openapi.yml
- filename: threads-api-read-and-manage-threads-retrieve-threads-profiles-api-openapi.yml
  format: yaml
  label: Threads Read And Manage Threads > Retrieve Threads Profiles API
  slug: threads-api-read-and-manage-threads-retrieve-threads-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threads-api/refs/heads/main/openapi/threads-api-read-and-manage-threads-retrieve-threads-profiles-api-openapi.yml
- filename: threads-api-troubleshooting-api-openapi.yml
  format: yaml
  label: Threads Troubleshooting API
  slug: threads-api-troubleshooting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/threads-api/refs/heads/main/openapi/threads-api-troubleshooting-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Threads Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Threads secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Threads
provider_slug: threads-api
scheme_count: 2
schemes:
- name: noauthAuth
  scheme: noauth
  sources:
  - openapi/threads-api-openapi.yml
  - openapi/threads-api.yml
  type: http
- name: oauth2Auth
  scheme: oauth2
  sources:
  - openapi/threads-api-openapi.yml
  - openapi/threads-api.yml
  type: http
slug: threads-api-authentication
source_filename: threads-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/threads-api-openapi.yml, openapi/threads-api.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: noauthAuth\n  type: http\n  scheme: noauth\n  sources:\n  - openapi/threads-api-openapi.yml\n  - openapi/threads-api.yml\n- name: oauth2Auth\n  type: http\n  scheme: oauth2\n  sources:\n  - openapi/threads-api-openapi.yml\n  - openapi/threads-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/threads-api/refs/heads/main/authentication/threads-api-authentication.yml
summary_line: http · 2 schemes
tags:
- Social
- Social Networks
- Meta
- Publishing
- Media
---
