---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cache-boost-com-auth-api-openapi.yml
  format: yaml
  label: CacheBoost Auth API
  slug: cache-boost-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cache-boost-com/openapi/cache-boost-com-auth-api-openapi.yml
- filename: cache-boost-com-boosts-api-openapi.yml
  format: yaml
  label: CacheBoost Boosts API
  slug: cache-boost-com-boosts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cache-boost-com/openapi/cache-boost-com-boosts-api-openapi.yml
- filename: cache-boost-com-runs-api-openapi.yml
  format: yaml
  label: CacheBoost Runs API
  slug: cache-boost-com-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cache-boost-com/openapi/cache-boost-com-runs-api-openapi.yml
- filename: cache-boost-com-sitemaps-api-openapi.yml
  format: yaml
  label: CacheBoost Sitemaps API
  slug: cache-boost-com-sitemaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cache-boost-com/openapi/cache-boost-com-sitemaps-api-openapi.yml
- filename: cache-boost-com-sites-api-openapi.yml
  format: yaml
  label: CacheBoost Sites API
  slug: cache-boost-com-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cache-boost-com/openapi/cache-boost-com-sites-api-openapi.yml
auth_types: []
description: Authentication for CacheBoost API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cache Boost Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: CacheBoost declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CacheBoost
provider_slug: cache-boost-com
scheme_count: 1
schemes:
- evidence: All API requests require a Bearer token.
  header: Authorization
  how_to_obtain: Create an API key in the profile page (https://app.cache-boost.com/profile) and copy the shown key.
  location: header
  name: Bearer
  scopes:
  - sites:read
  - sites:write
  - boosts:read
  - boosts:write
  - runs:read
  type: http-bearer
slug: cache-boost-com-authentication
source_filename: cache-boost-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.cache-boost.com/support/getting-started/authentication.md
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.cache-boost.com/support/getting-started/authentication.md\nsources:\n- https://www.cache-boost.com/support/getting-started/authentication.md\n- https://www.cache-boost.com/support/getting-started/introduction.md\n- https://www.cache-boost.com/support/getting-started/quickstart.md\ndescription: Authentication for CacheBoost API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: All API requests require a Bearer token.\n  location: header\n  header: Authorization\n  scopes:\n  - sites:read\n  - sites:write\n  - boosts:read\n  - boosts:write\n  - runs:read\n  how_to_obtain: Create an API key in the profile page (https://app.cache-boost.com/profile) and copy the shown key.\nnote: No OAuth2 flows or other authentication types are documented.\ndocs: https://www.cache-boost.com/support/getting-started/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/cache-boost-com/authentication/cache-boost-com-authentication.yml
summary_line: 1 scheme
tags:
- Cache
- Performance
- SEO
- WordPress
- CDN
---
