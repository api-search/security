---
anonymous_access: false
api_key_in: []
api_specs:
- filename: infiniteappsai-com-core-openapi-generated.yml
  format: yaml
  label: InfiniteApps core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteappsai-com/openapi/_ae-authored/infiniteappsai-com-core-openapi-generated.yml
- filename: infiniteappsai-com-forge-openapi-generated.yml
  format: yaml
  label: InfiniteApps forge API
  slug: forge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteappsai-com/openapi/_ae-authored/infiniteappsai-com-forge-openapi-generated.yml
- filename: infiniteappsai-com-getting-started-openapi-generated.yml
  format: yaml
  label: InfiniteApps getting started API
  slug: getting-started-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infiniteappsai-com/openapi/_ae-authored/infiniteappsai-com-getting-started-openapi-generated.yml
auth_types: []
description: Authentication methods for InfiniteApps Forge API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: InfiniteApps Authentication
name_suffix: Authentication
oauth_flows: []
overview: InfiniteApps declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: InfiniteApps
provider_slug: infiniteappsai-com
scheme_count: 1
schemes:
- evidence: Info Every request requires an API key in the X-API-Key header.
  header: X-API-Key
  how_to_obtain: Rotate keys through the dashboard or Doppler; keys are created per organization.
  location: header
  name: API Key
  type: apiKey
slug: infiniteappsai-com-authentication
source_filename: infiniteappsai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.infiniteappsai.com/docs/forge-api/auth-patterns
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.infiniteappsai.com/docs/forge-api/auth-patterns\nsources:\n- https://www.infiniteappsai.com/docs/forge-api/auth-patterns\n- https://www.infiniteappsai.com/docs/forge-api/overview\n- https://www.infiniteappsai.com/docs/getting-started/platform-overview\n- https://www.infiniteappsai.com/docs/getting-started/architecture\ndescription: Authentication methods for InfiniteApps Forge API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Info Every request requires an API key in the X-API-Key header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Rotate keys through the dashboard or Doppler; keys are created per organization.\nnote: No OAuth2, HTTP Bearer, or other authentication schemes are documented on the provided pages.\ndocs: https://www.infiniteappsai.com/docs/forge-api/auth-patterns\n"
source_yaml_url: https://artifacts.apis.io/infiniteappsai-com/authentication/infiniteappsai-com-authentication.yml
summary_line: 1 scheme
tags:
- SaaS Platform
- Multi-Tenant
- Billing
---
