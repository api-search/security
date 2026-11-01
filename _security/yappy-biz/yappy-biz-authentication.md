---
anonymous_access: false
api_key_in: []
api_specs:
- filename: yappy-biz-batch-api-openapi.yml
  format: yaml
  label: yappy-biz Batch API
  slug: yappy-biz-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-batch-api-openapi.yml
- filename: yappy-biz-commerce-api-openapi.yml
  format: yaml
  label: yappy-biz Commerce API
  slug: yappy-biz-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-commerce-api-openapi.yml
- filename: yappy-biz-discovery-api-openapi.yml
  format: yaml
  label: yappy-biz Discovery API
  slug: yappy-biz-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-discovery-api-openapi.yml
- filename: yappy-biz-documentation-api-openapi.yml
  format: yaml
  label: yappy-biz Documentation API
  slug: yappy-biz-documentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-documentation-api-openapi.yml
- filename: yappy-biz-exports-api-openapi.yml
  format: yaml
  label: yappy-biz Exports API
  slug: yappy-biz-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-exports-api-openapi.yml
- filename: yappy-biz-product-api-openapi.yml
  format: yaml
  label: yappy-biz Product API
  slug: yappy-biz-product-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-product-api-openapi.yml
- filename: yappy-biz-releases-api-openapi.yml
  format: yaml
  label: yappy-biz Releases API
  slug: yappy-biz-releases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-releases-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Yappy Biz Authentication
name_suffix: Authentication
oauth_flows: []
overview: yappy-biz declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: yappy-biz
provider_slug: yappy-biz
scheme_count: 2
schemes:
- bearerFormat: opaque
  description: Bearer token optional for read endpoints; required for higher limits and exports
  scheme: bearer
  type: http
- description: OAuth 2.1 with PKCE S256, dynamic client registration
  flows:
    clientCredentials:
      scopes:
        export:docs: Start and poll documentation export jobs
        read:docs: Read documentation pages and run searches
        read:faq: Read frequently asked questions
        read:pricing: Read pricing and plan data
        read:releases: Read release history and the current version
      tokenUrl: https://yappy.biz/oauth/token
  type: oauth2
slug: yappy-biz-authentication
source_filename: yappy-biz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://yappy.biz/developers/authentication.md\nschemes:\n  - type: http\n    scheme: bearer\n    description: \"Bearer token optional for read endpoints; required for higher limits and exports\"\n    bearerFormat: opaque\n  - type: oauth2\n    description: \"OAuth 2.1 with PKCE S256, dynamic client registration\"\n    flows:\n      clientCredentials:\n        tokenUrl: https://yappy.biz/oauth/token\n        scopes:\n          read:releases: \"Read release history and the current version\"\n          read:docs: \"Read documentation pages and run searches\"\n          read:pricing: \"Read pricing and plan data\"\n          read:faq: \"Read frequently asked questions\"\n          export:docs: \"Start and poll documentation export jobs\"\n"
source_yaml_url: https://artifacts.apis.io/yappy-biz/authentication/yappy-biz-authentication.yml
summary_line: 2 schemes
tags:
- Voice
- macOS
- Automation
- Accessibility
- Productivity
---
