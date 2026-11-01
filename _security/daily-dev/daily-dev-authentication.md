---
anonymous_access: false
api_key_in: []
api_specs:
- filename: daily-dev-bookmarks-api-openapi.yml
  format: yaml
  label: daily-dev Bookmarks API
  slug: daily-dev-bookmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-bookmarks-api-openapi.yml
- filename: daily-dev-custom-feeds-api-openapi.yml
  format: yaml
  label: daily-dev Custom Feeds API
  slug: daily-dev-custom-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-custom-feeds-api-openapi.yml
- filename: daily-dev-experiences-api-openapi.yml
  format: yaml
  label: daily-dev Experiences API
  slug: daily-dev-experiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-experiences-api-openapi.yml
- filename: daily-dev-feed-filters-api-openapi.yml
  format: yaml
  label: daily-dev Feed Filters API
  slug: daily-dev-feed-filters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-feed-filters-api-openapi.yml
- filename: daily-dev-feeds-api-openapi.yml
  format: yaml
  label: daily-dev Feeds API
  slug: daily-dev-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-feeds-api-openapi.yml
- filename: daily-dev-for-you-api-openapi.yml
  format: yaml
  label: daily-dev For You API
  slug: daily-dev-for-you-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-for-you-api-openapi.yml
- filename: daily-dev-notifications-api-openapi.yml
  format: yaml
  label: daily-dev Notifications API
  slug: daily-dev-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-notifications-api-openapi.yml
- filename: daily-dev-plugins-api-openapi.yml
  format: yaml
  label: daily-dev Plugins API
  slug: daily-dev-plugins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-plugins-api-openapi.yml
- filename: daily-dev-posts-api-openapi.yml
  format: yaml
  label: daily-dev Posts API
  slug: daily-dev-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-posts-api-openapi.yml
- filename: daily-dev-profile-api-openapi.yml
  format: yaml
  label: daily-dev Profile API
  slug: daily-dev-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-profile-api-openapi.yml
- filename: daily-dev-recommend-api-openapi.yml
  format: yaml
  label: daily-dev Recommend API
  slug: daily-dev-recommend-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-recommend-api-openapi.yml
- filename: daily-dev-search-api-openapi.yml
  format: yaml
  label: daily-dev Search API
  slug: daily-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-search-api-openapi.yml
- filename: daily-dev-stack-api-openapi.yml
  format: yaml
  label: daily-dev Stack API
  slug: daily-dev-stack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-stack-api-openapi.yml
- filename: daily-dev-tags-api-openapi.yml
  format: yaml
  label: daily-dev Tags API
  slug: daily-dev-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daily-dev/openapi/daily-dev-tags-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Daily Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: daily-dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: daily-dev
provider_slug: daily-dev
scheme_count: 2
schemes:
- description: Personal Access Token
  name: bearerAuth
  scheme: bearer
  type: http
- description: OAuth 2.0 authorization code flow with PKCE
  flows:
    authorizationCode:
      authorizationUrl: https://api.daily.dev/auth/oauth2/authorize
      scopes:
        read: Read your daily.dev data
        write: Change your daily.dev data
      tokenUrl: https://api.daily.dev/auth/oauth2/token
  type: oauth2
slug: daily-dev-authentication
source_filename: daily-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: https://api.daily.dev/public/v1/docs/json\nschemes:\n  - type: http\n    scheme: bearer\n    description: Personal Access Token\n    name: bearerAuth\n  - type: oauth2\n    description: OAuth 2.0 authorization code flow with PKCE\n    flows:\n      authorizationCode:\n        authorizationUrl: https://api.daily.dev/auth/oauth2/authorize\n        tokenUrl: https://api.daily.dev/auth/oauth2/token\n        scopes:\n          read: Read your daily.dev data\n          write: Change your daily.dev data\n"
source_yaml_url: https://artifacts.apis.io/daily-dev/authentication/daily-dev-authentication.yml
summary_line: 2 schemes
tags:
- Company
- DeveloperTools
- NewsAggregator
- AI
- Community
---
