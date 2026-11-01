---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: socialapis-account-api-openapi.yml
  format: yaml
  label: SocialAPIs Account API
  slug: socialapis-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-account-api-openapi.yml
- filename: socialapis-facebook-groups-api-openapi.yml
  format: yaml
  label: SocialAPIs Facebook Groups API
  slug: socialapis-facebook-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-facebook-groups-api-openapi.yml
- filename: socialapis-facebook-marketplace-api-openapi.yml
  format: yaml
  label: SocialAPIs Facebook Marketplace API
  slug: socialapis-facebook-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-facebook-marketplace-api-openapi.yml
- filename: socialapis-facebook-media-api-openapi.yml
  format: yaml
  label: SocialAPIs Facebook Media API
  slug: socialapis-facebook-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-facebook-media-api-openapi.yml
- filename: socialapis-facebook-pages-api-openapi.yml
  format: yaml
  label: SocialAPIs Facebook Pages API
  slug: socialapis-facebook-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-facebook-pages-api-openapi.yml
- filename: socialapis-facebook-posts-api-openapi.yml
  format: yaml
  label: SocialAPIs Facebook Posts API
  slug: socialapis-facebook-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-facebook-posts-api-openapi.yml
- filename: socialapis-facebook-search-api-openapi.yml
  format: yaml
  label: SocialAPIs Facebook Search API
  slug: socialapis-facebook-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-facebook-search-api-openapi.yml
- filename: socialapis-instagram-api-openapi.yml
  format: yaml
  label: SocialAPIs Instagram API
  slug: socialapis-instagram-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-instagram-api-openapi.yml
- filename: socialapis-meta-ads-library-api-openapi.yml
  format: yaml
  label: SocialAPIs Meta Ads Library API
  slug: socialapis-meta-ads-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-meta-ads-library-api-openapi.yml
- filename: socialapis-other-api-openapi.yml
  format: yaml
  label: SocialAPIs Other API
  slug: socialapis-other-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/socialapis/openapi/socialapis-other-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Socialapis Authentication
name_suffix: Authentication
oauth_flows: []
overview: SocialAPIs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SocialAPIs
provider_slug: socialapis
scheme_count: 1
schemes:
- description: Your API key from https://socialapis.io/dashboard
  in: header
  name: ApiKey
  parameter: x-api-token
  sources:
  - openapi/socialapis-openapi.json
  type: apiKey
slug: socialapis-authentication
source_filename: socialapis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: derived\nsource: openapi/socialapis-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-token\n  description: Your API key from https://socialapis.io/dashboard\n  sources:\n  - openapi/socialapis-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/socialapis/authentication/socialapis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Social Media
- Data
- Developers
---
