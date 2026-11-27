---
anonymous_access: false
api_key_in: []
api_specs:
- filename: groundroute-ai-admin-api-openapi.yml
  format: yaml
  label: GroundRoute AI Admin API
  slug: groundroute-ai-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-admin-api-openapi.yml
- filename: groundroute-ai-analytics-api-openapi.yml
  format: yaml
  label: GroundRoute AI Analytics API
  slug: groundroute-ai-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-analytics-api-openapi.yml
- filename: groundroute-ai-billing-api-openapi.yml
  format: yaml
  label: GroundRoute AI Billing API
  slug: groundroute-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-billing-api-openapi.yml
- filename: groundroute-ai-cards-api-openapi.yml
  format: yaml
  label: GroundRoute AI Cards API
  slug: groundroute-ai-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-cards-api-openapi.yml
- filename: groundroute-ai-console-api-openapi.yml
  format: yaml
  label: GroundRoute AI Console API
  slug: groundroute-ai-console-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-console-api-openapi.yml
- filename: groundroute-ai-console-auth-api-openapi.yml
  format: yaml
  label: GroundRoute AI Console Auth API
  slug: groundroute-ai-console-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-console-auth-api-openapi.yml
- filename: groundroute-ai-console-billing-api-openapi.yml
  format: yaml
  label: GroundRoute AI Console Billing API
  slug: groundroute-ai-console-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-console-billing-api-openapi.yml
- filename: groundroute-ai-console-byok-api-openapi.yml
  format: yaml
  label: GroundRoute AI Console Byok API
  slug: groundroute-ai-console-byok-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-console-byok-api-openapi.yml
- filename: groundroute-ai-console-keys-api-openapi.yml
  format: yaml
  label: GroundRoute AI Console Keys API
  slug: groundroute-ai-console-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-console-keys-api-openapi.yml
- filename: groundroute-ai-funnel-api-openapi.yml
  format: yaml
  label: GroundRoute AI Funnel API
  slug: groundroute-ai-funnel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-funnel-api-openapi.yml
- filename: groundroute-ai-healthz-api-openapi.yml
  format: yaml
  label: GroundRoute AI Healthz API
  slug: groundroute-ai-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-healthz-api-openapi.yml
- filename: groundroute-ai-metrics-api-openapi.yml
  format: yaml
  label: GroundRoute AI Metrics API
  slug: groundroute-ai-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-metrics-api-openapi.yml
- filename: groundroute-ai-playground-api-openapi.yml
  format: yaml
  label: GroundRoute AI Playground API
  slug: groundroute-ai-playground-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-playground-api-openapi.yml
- filename: groundroute-ai-readyz-api-openapi.yml
  format: yaml
  label: GroundRoute AI Readyz API
  slug: groundroute-ai-readyz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-readyz-api-openapi.yml
- filename: groundroute-ai-referral-api-openapi.yml
  format: yaml
  label: GroundRoute AI Referral API
  slug: groundroute-ai-referral-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-referral-api-openapi.yml
- filename: groundroute-ai-search-api-openapi.yml
  format: yaml
  label: GroundRoute AI Search API
  slug: groundroute-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-search-api-openapi.yml
- filename: groundroute-ai-signup-offer-api-openapi.yml
  format: yaml
  label: GroundRoute AI Signup Offer API
  slug: groundroute-ai-signup-offer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-signup-offer-api-openapi.yml
- filename: groundroute-ai-usage-api-openapi.yml
  format: yaml
  label: GroundRoute AI Usage API
  slug: groundroute-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-usage-api-openapi.yml
- filename: groundroute-ai-well-known-api-openapi.yml
  format: yaml
  label: GroundRoute AI .well Known API
  slug: groundroute-ai-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groundroute-ai/openapi/groundroute-ai-well-known-api-openapi.yml
auth_types: []
description: Authentication uses an API key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: GroundRoute AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: GroundRoute AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GroundRoute AI
provider_slug: groundroute-ai
scheme_count: 1
schemes:
- evidence: Every request to the GroundRoute API authenticates with an API key sent as a Bearer token.
  header: Authorization
  how_to_obtain: Create an API key in the console; the plaintext key is shown once and must be stored securely.
  location: header
  name: Authorization
  type: apiKey
slug: groundroute-ai-authentication
source_filename: groundroute-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://groundroute.ai/docs/authentication
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://groundroute.ai/docs/authentication\nsources:\n- https://groundroute.ai/docs/authentication\n- https://groundroute.ai/docs/quickstart\ndescription: Authentication uses an API key sent as a Bearer token in the Authorization header.\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: Every request to the GroundRoute API authenticates with an API key sent as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the console; the plaintext key is shown once and must be stored securely.\nnote: No OAuth2, http-bearer, http-basic, JWT, HMAC, mTLS, or other schemes are documented.\ndocs: https://groundroute.ai/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/groundroute-ai/authentication/groundroute-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Search
- Routing
- Cost-Saving
- Analytics
---
