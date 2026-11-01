---
anonymous_access: false
api_key_in: []
api_specs:
- filename: beatapi-account-api-openapi.yml
  format: yaml
  label: BeatAPI Account API
  slug: beatapi-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-account-api-openapi.yml
- filename: beatapi-capabilities-api-openapi.yml
  format: yaml
  label: BeatAPI Capabilities API
  slug: beatapi-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-capabilities-api-openapi.yml
- filename: beatapi-decisions-api-openapi.yml
  format: yaml
  label: BeatAPI Decisions API
  slug: beatapi-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-decisions-api-openapi.yml
- filename: beatapi-ecommerce-video-api-openapi.yml
  format: yaml
  label: BeatAPI Ecommerce Video API
  slug: beatapi-ecommerce-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-ecommerce-video-api-openapi.yml
- filename: beatapi-effects-api-openapi.yml
  format: yaml
  label: BeatAPI Effects API
  slug: beatapi-effects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-effects-api-openapi.yml
- filename: beatapi-files-api-openapi.yml
  format: yaml
  label: BeatAPI Files API
  slug: beatapi-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-files-api-openapi.yml
- filename: beatapi-generation-api-openapi.yml
  format: yaml
  label: BeatAPI Generation API
  slug: beatapi-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-generation-api-openapi.yml
- filename: beatapi-music-video-api-openapi.yml
  format: yaml
  label: BeatAPI Music Video API
  slug: beatapi-music-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-music-video-api-openapi.yml
- filename: beatapi-realtime-video-api-openapi.yml
  format: yaml
  label: BeatAPI Realtime Video API
  slug: beatapi-realtime-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-realtime-video-api-openapi.yml
- filename: beatapi-social-data-api-openapi.yml
  format: yaml
  label: BeatAPI Social Data API
  slug: beatapi-social-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-social-data-api-openapi.yml
- filename: beatapi-tasks-api-openapi.yml
  format: yaml
  label: BeatAPI Tasks API
  slug: beatapi-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-tasks-api-openapi.yml
- filename: beatapi-text-api-openapi.yml
  format: yaml
  label: BeatAPI Text API
  slug: beatapi-text-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-text-api-openapi.yml
- filename: beatapi-usage-api-openapi.yml
  format: yaml
  label: BeatAPI Usage API
  slug: beatapi-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-usage-api-openapi.yml
- filename: beatapi-video-analysis-api-openapi.yml
  format: yaml
  label: BeatAPI Video Analysis API
  slug: beatapi-video-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-video-analysis-api-openapi.yml
- filename: beatapi-web-search-api-openapi.yml
  format: yaml
  label: BeatAPI Web Search API
  slug: beatapi-web-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-web-search-api-openapi.yml
- filename: beatapi-webhooks-api-openapi.yml
  format: yaml
  label: BeatAPI Webhooks API
  slug: beatapi-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-webhooks-api-openapi.yml
- filename: beatapi-workflows-api-openapi.yml
  format: yaml
  label: BeatAPI Workflows API
  slug: beatapi-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/beatapi/openapi/beatapi-workflows-api-openapi.yml
auth_types: []
description: Authentication methods for BeatAPI
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Beatapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: BeatAPI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BeatAPI
provider_slug: beatapi
scheme_count: 2
schemes:
- evidence: 'The header is the only correct place: Authorization: Bearer <key> .'
  header: Authorization
  how_to_obtain: Create a key in Dashboard → API Keys and copy it when shown.
  location: header
  name: API Key
  type: http-bearer
- evidence: 'Send the token as Authorization: Bearer <token> .'
  header: Authorization
  how_to_obtain: Sign in to the Dashboard, open Account security, choose Create personal token, set permissions and expiry, then copy the token.
  location: header
  name: Personal Access Token
  type: http-bearer
slug: beatapi-authentication
source_filename: beatapi-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.beatapi.io/faq/keys-security
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.beatapi.io/faq/keys-security\nsources:\n- https://docs.beatapi.io/faq/keys-security\n- https://docs.beatapi.io/personal-access-token\ndescription: Authentication methods for BeatAPI\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'The header is the only correct place: Authorization: Bearer <key> .'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Dashboard → API Keys and copy it when shown.\n- type: http-bearer\n  name: Personal Access Token\n  evidence: 'Send the token as Authorization: Bearer <token> .'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in to the Dashboard, open Account security, choose Create personal token, set permissions and expiry, then copy the token.\ndocs: https://docs.beatapi.io/faq/keys-security\n"
source_yaml_url: https://artifacts.apis.io/beatapi/authentication/beatapi-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Platform
- Unified-API
- Data-Integration
---
