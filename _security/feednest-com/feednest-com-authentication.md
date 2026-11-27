---
anonymous_access: false
api_key_in: []
api_specs:
- filename: feednest-com-ai-api-openapi.yml
  format: yaml
  label: FeedNest AI API
  slug: feednest-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feednest-com/openapi/feednest-com-ai-api-openapi.yml
- filename: feednest-com-articles-api-openapi.yml
  format: yaml
  label: FeedNest Articles API
  slug: feednest-com-articles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feednest-com/openapi/feednest-com-articles-api-openapi.yml
- filename: feednest-com-feeds-api-openapi.yml
  format: yaml
  label: FeedNest Feeds API
  slug: feednest-com-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feednest-com/openapi/feednest-com-feeds-api-openapi.yml
- filename: feednest-com-folders-api-openapi.yml
  format: yaml
  label: FeedNest Folders API
  slug: feednest-com-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feednest-com/openapi/feednest-com-folders-api-openapi.yml
- filename: feednest-com-health-api-openapi.yml
  format: yaml
  label: FeedNest Health API
  slug: feednest-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feednest-com/openapi/feednest-com-health-api-openapi.yml
- filename: feednest-com-highlights-api-openapi.yml
  format: yaml
  label: FeedNest Highlights API
  slug: feednest-com-highlights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feednest-com/openapi/feednest-com-highlights-api-openapi.yml
- filename: feednest-com-notes-api-openapi.yml
  format: yaml
  label: FeedNest Notes API
  slug: feednest-com-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feednest-com/openapi/feednest-com-notes-api-openapi.yml
- filename: feednest-com-output-feeds-api-openapi.yml
  format: yaml
  label: FeedNest Output Feeds API
  slug: feednest-com-output-feeds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feednest-com/openapi/feednest-com-output-feeds-api-openapi.yml
- filename: feednest-com-saved-api-openapi.yml
  format: yaml
  label: FeedNest Saved API
  slug: feednest-com-saved-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feednest-com/openapi/feednest-com-saved-api-openapi.yml
- filename: feednest-com-stats-api-openapi.yml
  format: yaml
  label: FeedNest Stats API
  slug: feednest-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feednest-com/openapi/feednest-com-stats-api-openapi.yml
- filename: feednest-com-tags-api-openapi.yml
  format: yaml
  label: FeedNest Tags API
  slug: feednest-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feednest-com/openapi/feednest-com-tags-api-openapi.yml
auth_types: []
description: FeedNest uses API keys presented as Bearer tokens.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FeedNest Authentication
name_suffix: Authentication
oauth_flows: []
overview: FeedNest declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FeedNest
provider_slug: feednest-com
scheme_count: 1
schemes:
- evidence: Authentication Bearer token in Authorization header
  header: Authorization
  how_to_obtain: Create an API key in Settings → Developer API; the key is shown once and used as the Bearer token.
  location: header
  name: Bearer token
  type: http-bearer
slug: feednest-com-authentication
source_filename: feednest-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.feednest.com/api-keys
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.feednest.com/api-keys\nsources:\n- https://docs.feednest.com/api-keys\n- https://docs.feednest.com/api-keys\n- https://docs.feednest.com/connect/general\ndescription: FeedNest uses API keys presented as Bearer tokens.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Authentication Bearer token in Authorization header\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings → Developer API; the key is shown once and used as the Bearer token.\nnote: No OAuth2, apiKey, or other authentication schemes are documented.\ndocs: https://docs.feednest.com/api-keys\n"
source_yaml_url: https://artifacts.apis.io/feednest-com/authentication/feednest-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- News
- Aggregation
- Privacy
- Productivity
- Company
---
