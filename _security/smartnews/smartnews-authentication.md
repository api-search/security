---
api_key_in: []
api_specs:
- filename: smartnews-ad-api-openapi.yml
  format: yaml
  label: SmartNews ad API
  slug: smartnews-ad-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-ad-api-openapi.yml
- filename: smartnews-ad-group-api-openapi.yml
  format: yaml
  label: SmartNews ad-group API
  slug: smartnews-ad-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-ad-group-api-openapi.yml
- filename: smartnews-article-category-api-openapi.yml
  format: yaml
  label: SmartNews article category API
  slug: smartnews-article-category-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-article-category-api-openapi.yml
- filename: smartnews-campaign-api-openapi.yml
  format: yaml
  label: SmartNews campaign API
  slug: smartnews-campaign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-campaign-api-openapi.yml
- filename: smartnews-catalog-api-openapi.yml
  format: yaml
  label: SmartNews catalog API
  slug: smartnews-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-catalog-api-openapi.yml
- filename: smartnews-channel-alias-label-api-openapi.yml
  format: yaml
  label: SmartNews channel alias label API
  slug: smartnews-channel-alias-label-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-channel-alias-label-api-openapi.yml
- filename: smartnews-custom-audience-api-openapi.yml
  format: yaml
  label: SmartNews custom-audience API
  slug: smartnews-custom-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-custom-audience-api-openapi.yml
- filename: smartnews-developer-app-api-openapi.yml
  format: yaml
  label: SmartNews developer-app API
  slug: smartnews-developer-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-developer-app-api-openapi.yml
- filename: smartnews-insights-api-openapi.yml
  format: yaml
  label: SmartNews insights API
  slug: smartnews-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-insights-api-openapi.yml
- filename: smartnews-interests-api-openapi.yml
  format: yaml
  label: SmartNews interests API
  slug: smartnews-interests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-interests-api-openapi.yml
- filename: smartnews-locations-api-openapi.yml
  format: yaml
  label: SmartNews locations API
  slug: smartnews-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-locations-api-openapi.yml
- filename: smartnews-media-file-api-openapi.yml
  format: yaml
  label: SmartNews media-file API
  slug: smartnews-media-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-media-file-api-openapi.yml
- filename: smartnews-oauth-api-openapi.yml
  format: yaml
  label: SmartNews oauth API
  slug: smartnews-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-oauth-api-openapi.yml
- filename: smartnews-pixel-api-openapi.yml
  format: yaml
  label: SmartNews pixel API
  slug: smartnews-pixel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-pixel-api-openapi.yml
- filename: smartnews-smart-view-article-keyword-api-openapi.yml
  format: yaml
  label: SmartNews smart view article keyword API
  slug: smartnews-smart-view-article-keyword-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/openapi/smartnews-smart-view-article-keyword-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Smartnews Authentication
name_suffix: Authentication
oauth_flows: []
overview: SmartNews secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SmartNews
provider_slug: smartnews
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/smartnews-ad-api-openapi.yml
  - openapi/smartnews-ad-group-api-openapi.yml
  - openapi/smartnews-article-category-api-openapi.yml
  - openapi/smartnews-campaign-api-openapi.yml
  - openapi/smartnews-catalog-api-openapi.yml
  - openapi/smartnews-channel-alias-label-api-openapi.yml
  - openapi/smartnews-custom-audience-api-openapi.yml
  - openapi/smartnews-developer-app-api-openapi.yml
  - openapi/smartnews-insights-api-openapi.yml
  - openapi/smartnews-interests-api-openapi.yml
  - openapi/smartnews-locations-api-openapi.yml
  - openapi/smartnews-media-file-api-openapi.yml
  - openapi/smartnews-oauth-api-openapi.yml
  - openapi/smartnews-pixel-api-openapi.yml
  - openapi/smartnews-smart-view-article-keyword-api-openapi.yml
  type: http
slug: smartnews-authentication
source_filename: smartnews-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/smartnews-ad-api-openapi.yml, openapi/smartnews-ad-group-api-openapi.yml, openapi/smartnews-article-category-api-openapi.yml,\n  openapi/smartnews-campaign-api-openapi.yml, openapi/smartnews-catalog-api-openapi.yml, openapi/smartnews-channel-alias-label-api-openapi.yml,\n  openapi/smartnews-custom-audience-api-openapi.yml, openapi/smartnews-developer-app-api-openapi.yml,\n  openapi/smartnews-insights-api-openapi.yml, openapi/smartnews-interests-api-openapi.yml, openapi/smartnews-locations-api-openapi.yml,\n  openapi/smartnews-media-file-api-openapi.yml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/smartnews-ad-api-openapi.yml\n  - openapi/smartnews-ad-group-api-openapi.yml\n  - openapi/smartnews-article-category-api-openapi.yml\n  - openapi/smartnews-campaign-api-openapi.yml\n  - openapi/smartnews-catalog-api-openapi.yml\n\
  \  - openapi/smartnews-channel-alias-label-api-openapi.yml\n  - openapi/smartnews-custom-audience-api-openapi.yml\n  - openapi/smartnews-developer-app-api-openapi.yml\n  - openapi/smartnews-insights-api-openapi.yml\n  - openapi/smartnews-interests-api-openapi.yml\n  - openapi/smartnews-locations-api-openapi.yml\n  - openapi/smartnews-media-file-api-openapi.yml\n  - openapi/smartnews-oauth-api-openapi.yml\n  - openapi/smartnews-pixel-api-openapi.yml\n  - openapi/smartnews-smart-view-article-keyword-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartnews/refs/heads/main/authentication/smartnews-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- News
- Advertising
- AdTech
- Marketing
- Media
- Campaign Management
---
