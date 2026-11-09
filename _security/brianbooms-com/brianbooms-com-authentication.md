---
anonymous_access: false
api_key_in: []
api_specs:
- filename: brianbooms-com-ascendency-api-openapi.yml
  format: yaml
  label: Brian Booms Ascendency API
  slug: brianbooms-com-ascendency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-ascendency-api-openapi.yml
- filename: brianbooms-com-btc-api-openapi.yml
  format: yaml
  label: Brian Booms Btc API
  slug: brianbooms-com-btc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-btc-api-openapi.yml
- filename: brianbooms-com-buy-api-openapi.yml
  format: yaml
  label: Brian Booms Buy API
  slug: brianbooms-com-buy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-buy-api-openapi.yml
- filename: brianbooms-com-catalog-api-openapi.yml
  format: yaml
  label: Brian Booms Catalog API
  slug: brianbooms-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-catalog-api-openapi.yml
- filename: brianbooms-com-clinic-api-openapi.yml
  format: yaml
  label: Brian Booms Clinic API
  slug: brianbooms-com-clinic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-clinic-api-openapi.yml
- filename: brianbooms-com-data-api-openapi.yml
  format: yaml
  label: Brian Booms Data API
  slug: brianbooms-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-data-api-openapi.yml
- filename: brianbooms-com-health-api-openapi.yml
  format: yaml
  label: Brian Booms Health API
  slug: brianbooms-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-health-api-openapi.yml
- filename: brianbooms-com-inquiry-api-openapi.yml
  format: yaml
  label: Brian Booms Inquiry API
  slug: brianbooms-com-inquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-inquiry-api-openapi.yml
- filename: brianbooms-com-license-api-openapi.yml
  format: yaml
  label: Brian Booms License API
  slug: brianbooms-com-license-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-license-api-openapi.yml
- filename: brianbooms-com-lyrics-api-openapi.yml
  format: yaml
  label: Brian Booms Lyrics API
  slug: brianbooms-com-lyrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-lyrics-api-openapi.yml
- filename: brianbooms-com-merch-kit-api-openapi.yml
  format: yaml
  label: Brian Booms Merch Kit API
  slug: brianbooms-com-merch-kit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-merch-kit-api-openapi.yml
- filename: brianbooms-com-playlist-api-openapi.yml
  format: yaml
  label: Brian Booms Playlist API
  slug: brianbooms-com-playlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-playlist-api-openapi.yml
- filename: brianbooms-com-press-kit-api-openapi.yml
  format: yaml
  label: Brian Booms Press Kit API
  slug: brianbooms-com-press-kit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-press-kit-api-openapi.yml
- filename: brianbooms-com-rail-api-openapi.yml
  format: yaml
  label: Brian Booms Rail API
  slug: brianbooms-com-rail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-rail-api-openapi.yml
- filename: brianbooms-com-research-api-openapi.yml
  format: yaml
  label: Brian Booms Research API
  slug: brianbooms-com-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-research-api-openapi.yml
- filename: brianbooms-com-rewards-api-openapi.yml
  format: yaml
  label: Brian Booms Rewards API
  slug: brianbooms-com-rewards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-rewards-api-openapi.yml
- filename: brianbooms-com-sleep-api-openapi.yml
  format: yaml
  label: Brian Booms Sleep API
  slug: brianbooms-com-sleep-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-sleep-api-openapi.yml
- filename: brianbooms-com-tips-api-openapi.yml
  format: yaml
  label: Brian Booms Tips API
  slug: brianbooms-com-tips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-tips-api-openapi.yml
- filename: brianbooms-com-tools-api-openapi.yml
  format: yaml
  label: Brian Booms Tools API
  slug: brianbooms-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/brianbooms-com/openapi/brianbooms-com-tools-api-openapi.yml
auth_types: []
description: Authentication for Synthetic Universe Data APIs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Brianbooms Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brian Booms declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Brian Booms
provider_slug: brianbooms-com
scheme_count: 1
schemes:
- evidence: You retry the same URL with the payment payload in the X-PAYMENT header.
  header: X-PAYMENT
  how_to_obtain: From your own wallet using the x402 SDK or manual signing to create a base64 payment payload.
  location: header
  name: X-PAYMENT
  type: other
slug: brianbooms-com-authentication
source_filename: brianbooms-com-authentication.yml
source_heading: Authentication Profile
source_url: https://brianbooms.com/tools/token-estimator/
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://brianbooms.com/tools/token-estimator/\nsources:\n- https://brianbooms.com/tools/token-estimator/\n- https://brianbooms.com/blog/10-hour-sleep-music-setup/\n- https://brianbooms.com/quickstart/\ndescription: Authentication for Synthetic Universe Data APIs\nschemes:\n- type: other\n  name: X-PAYMENT\n  evidence: You retry the same URL with the payment payload in the X-PAYMENT header.\n  location: header\n  header: X-PAYMENT\n  how_to_obtain: From your own wallet using the x402 SDK or manual signing to create a base64 payment payload.\ndocs: https://brianbooms.com/tools/token-estimator/\n"
source_yaml_url: https://artifacts.apis.io/brianbooms-com/authentication/brianbooms-com-authentication.yml
summary_line: 1 scheme
tags:
- Music
- Ambient
- Sleep
- Meditation
- Artificial Intelligence
---
