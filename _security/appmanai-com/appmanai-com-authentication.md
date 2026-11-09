---
anonymous_access: false
api_key_in: []
api_specs:
- filename: appmanai-com-app-metadata-api-openapi.yml
  format: yaml
  label: AppManAi App Metadata API
  slug: appmanai-com-app-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmanai-com/openapi/appmanai-com-app-metadata-api-openapi.yml
- filename: appmanai-com-app-metrics-api-openapi.yml
  format: yaml
  label: AppManAi App Metrics API
  slug: appmanai-com-app-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmanai-com/openapi/appmanai-com-app-metrics-api-openapi.yml
- filename: appmanai-com-app-reviews-api-openapi.yml
  format: yaml
  label: AppManAi App Reviews API
  slug: appmanai-com-app-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmanai-com/openapi/appmanai-com-app-reviews-api-openapi.yml
- filename: appmanai-com-app-search-api-openapi.yml
  format: yaml
  label: AppManAi App Search API
  slug: appmanai-com-app-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appmanai-com/openapi/appmanai-com-app-search-api-openapi.yml
auth_types: []
description: Authentication schemes for AppManAi
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Appmanai Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppManAi declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AppManAi
provider_slug: appmanai-com
scheme_count: 1
schemes:
- evidence: 'Every request to the HTTP API authenticates with a Bearer API key. Send it in the Authorization header:'
  header: Authorization
  how_to_obtain: Create a key in your dashboard.
  location: header
  name: Bearer
  type: http-bearer
slug: appmanai-com-authentication
source_filename: appmanai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://appmanai.com/docs/guide/authentication.html
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://appmanai.com/docs/guide/authentication.html\nsources:\n- https://appmanai.com/docs/guide/authentication.html\n- https://appmanai.com/docs/guide/quickstart.html\ndescription: Authentication schemes for AppManAi\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request to the HTTP API authenticates with a Bearer API key. Send it in the Authorization header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in your dashboard.\ndocs: https://appmanai.com/docs/guide/authentication.html\n"
source_yaml_url: https://artifacts.apis.io/appmanai-com/authentication/appmanai-com-authentication.yml
summary_line: 1 scheme
tags:
- App Store Data
- Google Play Data
- ASO
- Data API
- App Intelligence
---
