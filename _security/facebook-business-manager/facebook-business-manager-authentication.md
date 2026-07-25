---
api_key_in: []
api_specs:
- filename: facebook-business-manager-ad-accounts-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Accounts API
  slug: facebook-business-manager-ad-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-accounts-api-openapi.yml
- filename: facebook-business-manager-ad-creatives-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Creatives API
  slug: facebook-business-manager-ad-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-creatives-api-openapi.yml
- filename: facebook-business-manager-ad-images-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Images API
  slug: facebook-business-manager-ad-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-images-api-openapi.yml
- filename: facebook-business-manager-ad-sets-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ad Sets API
  slug: facebook-business-manager-ad-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ad-sets-api-openapi.yml
- filename: facebook-business-manager-ads-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Ads API
  slug: facebook-business-manager-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-ads-api-openapi.yml
- filename: facebook-business-manager-campaigns-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Campaigns API
  slug: facebook-business-manager-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-campaigns-api-openapi.yml
- filename: facebook-business-manager-comments-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Comments API
  slug: facebook-business-manager-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-comments-api-openapi.yml
- filename: facebook-business-manager-custom-audiences-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Custom Audiences API
  slug: facebook-business-manager-custom-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-custom-audiences-api-openapi.yml
- filename: facebook-business-manager-insights-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Insights API
  slug: facebook-business-manager-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-insights-api-openapi.yml
- filename: facebook-business-manager-page-insights-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Page Insights API
  slug: facebook-business-manager-page-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-page-insights-api-openapi.yml
- filename: facebook-business-manager-pages-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Pages API
  slug: facebook-business-manager-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-pages-api-openapi.yml
- filename: facebook-business-manager-photos-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Photos API
  slug: facebook-business-manager-photos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-photos-api-openapi.yml
- filename: facebook-business-manager-posts-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Posts API
  slug: facebook-business-manager-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-posts-api-openapi.yml
- filename: facebook-business-manager-videos-api-openapi.yml
  format: yaml
  label: Facebook Business Manager Videos API
  slug: facebook-business-manager-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/openapi/facebook-business-manager-videos-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Facebook Business Manager Authentication
name_suffix: Authentication
oauth_flows: []
overview: Facebook Business Manager secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Facebook Business Manager
provider_slug: facebook-business-manager
scheme_count: 1
schemes:
- description: OAuth 2.0 access token with ads_management or ads_read permissions. Obtain tokens via the Facebook Login flow.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/facebook-marketing-openapi.yml
  - openapi/facebook-pages-openapi.yml
  type: http
slug: facebook-business-manager-authentication
source_filename: facebook-business-manager-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/facebook-marketing-openapi.yml, openapi/facebook-pages-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 access token with ads_management or ads_read permissions. Obtain tokens\n    via the Facebook Login flow.\n  sources:\n  - openapi/facebook-marketing-openapi.yml\n  - openapi/facebook-pages-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook-business-manager/refs/heads/main/authentication/facebook-business-manager-authentication.yml
summary_line: http · 1 scheme
tags:
- Advertising
- Analytics
- Business Management
- Marketing
- Social Media
---
