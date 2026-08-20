---
api_key_in: []
api_specs:
- filename: facebook-ad-accounts-api-openapi.yml
  format: yaml
  label: Facebook Ad Accounts API
  slug: facebook-ad-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-ad-accounts-api-openapi.yml
- filename: facebook-ad-sets-api-openapi.yml
  format: yaml
  label: Facebook Ad Sets API
  slug: facebook-ad-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-ad-sets-api-openapi.yml
- filename: facebook-ads-api-openapi.yml
  format: yaml
  label: Facebook Ads API
  slug: facebook-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-ads-api-openapi.yml
- filename: facebook-audiences-api-openapi.yml
  format: yaml
  label: Facebook Audiences API
  slug: facebook-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-audiences-api-openapi.yml
- filename: facebook-authentication-api-openapi.yml
  format: yaml
  label: Facebook Authentication API
  slug: facebook-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-authentication-api-openapi.yml
- filename: facebook-campaigns-api-openapi.yml
  format: yaml
  label: Facebook Campaigns API
  slug: facebook-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-campaigns-api-openapi.yml
- filename: facebook-comments-api-openapi.yml
  format: yaml
  label: Facebook Comments API
  slug: facebook-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-comments-api-openapi.yml
- filename: facebook-conversations-api-openapi.yml
  format: yaml
  label: Facebook Conversations API
  slug: facebook-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-conversations-api-openapi.yml
- filename: facebook-insights-api-openapi.yml
  format: yaml
  label: Facebook Insights API
  slug: facebook-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-insights-api-openapi.yml
- filename: facebook-media-api-openapi.yml
  format: yaml
  label: Facebook Media API
  slug: facebook-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-media-api-openapi.yml
- filename: facebook-messages-api-openapi.yml
  format: yaml
  label: Facebook Messages API
  slug: facebook-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-messages-api-openapi.yml
- filename: facebook-pages-api-openapi.yml
  format: yaml
  label: Facebook Pages API
  slug: facebook-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-pages-api-openapi.yml
- filename: facebook-phone-numbers-api-openapi.yml
  format: yaml
  label: Facebook Phone Numbers API
  slug: facebook-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-phone-numbers-api-openapi.yml
- filename: facebook-photos-api-openapi.yml
  format: yaml
  label: Facebook Photos API
  slug: facebook-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-photos-api-openapi.yml
- filename: facebook-posts-api-openapi.yml
  format: yaml
  label: Facebook Posts API
  slug: facebook-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-posts-api-openapi.yml
- filename: facebook-profile-api-openapi.yml
  format: yaml
  label: Facebook Profile API
  slug: facebook-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-profile-api-openapi.yml
- filename: facebook-publishing-api-openapi.yml
  format: yaml
  label: Facebook Publishing API
  slug: facebook-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-publishing-api-openapi.yml
- filename: facebook-replies-api-openapi.yml
  format: yaml
  label: Facebook Replies API
  slug: facebook-replies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-replies-api-openapi.yml
- filename: facebook-tags-api-openapi.yml
  format: yaml
  label: Facebook Tags API
  slug: facebook-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-tags-api-openapi.yml
- filename: facebook-templates-api-openapi.yml
  format: yaml
  label: Facebook Templates API
  slug: facebook-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-templates-api-openapi.yml
- filename: facebook-users-api-openapi.yml
  format: yaml
  label: Facebook Users API
  slug: facebook-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/openapi/facebook-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Facebook Authentication
name_suffix: Authentication
oauth_flows: []
overview: Facebook secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Facebook
provider_slug: facebook
scheme_count: 1
schemes:
- description: OAuth 2.0 access token for Facebook Graph API.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/facebook-graph-api.yaml
  - openapi/facebook-instagram-api.yaml
  - openapi/facebook-marketing-api.yaml
  - openapi/facebook-messenger-api.yaml
  - openapi/facebook-threads-api.yaml
  - openapi/facebook-whatsapp-api.yaml
  type: http
slug: facebook-authentication
source_filename: facebook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/facebook-graph-api.yaml, openapi/facebook-instagram-api.yaml, openapi/facebook-marketing-api.yaml,\n  openapi/facebook-messenger-api.yaml, openapi/facebook-threads-api.yaml, openapi/facebook-whatsapp-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token for Facebook Graph API.\n  sources:\n  - openapi/facebook-graph-api.yaml\n  - openapi/facebook-instagram-api.yaml\n  - openapi/facebook-marketing-api.yaml\n  - openapi/facebook-messenger-api.yaml\n  - openapi/facebook-threads-api.yaml\n  - openapi/facebook-whatsapp-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook/refs/heads/main/authentication/facebook-authentication.yml
summary_line: http · 1 scheme
tags:
- Fortune 500
- Advertising
- Content Publishing
- Messaging
- Social-Media
- Social Networking
---
