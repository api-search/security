---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: nothumansearch-ai-action-interests-api-openapi.yml
  format: yaml
  label: Not Human Search Action Interests API
  slug: nothumansearch-ai-action-interests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-action-interests-api-openapi.yml
- filename: nothumansearch-ai-action-receipts-api-openapi.yml
  format: yaml
  label: Not Human Search Action Receipts API
  slug: nothumansearch-ai-action-receipts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-action-receipts-api-openapi.yml
- filename: nothumansearch-ai-action-tickets-api-openapi.yml
  format: yaml
  label: Not Human Search Action Tickets API
  slug: nothumansearch-ai-action-tickets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-action-tickets-api-openapi.yml
- filename: nothumansearch-ai-api-keys-api-openapi.yml
  format: yaml
  label: Not Human Search Api Keys API
  slug: nothumansearch-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-api-keys-api-openapi.yml
- filename: nothumansearch-ai-catalog-api-openapi.yml
  format: yaml
  label: Not Human Search Catalog API
  slug: nothumansearch-ai-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-catalog-api-openapi.yml
- filename: nothumansearch-ai-categories-api-openapi.yml
  format: yaml
  label: Not Human Search Categories API
  slug: nothumansearch-ai-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-categories-api-openapi.yml
- filename: nothumansearch-ai-check-api-openapi.yml
  format: yaml
  label: Not Human Search Check API
  slug: nothumansearch-ai-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-check-api-openapi.yml
- filename: nothumansearch-ai-checkout-api-openapi.yml
  format: yaml
  label: Not Human Search Checkout API
  slug: nothumansearch-ai-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-checkout-api-openapi.yml
- filename: nothumansearch-ai-monitor-api-openapi.yml
  format: yaml
  label: Not Human Search Monitor API
  slug: nothumansearch-ai-monitor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-monitor-api-openapi.yml
- filename: nothumansearch-ai-not-human-search-api-api-openapi.yml
  format: yaml
  label: Not Human Search Not Human Search API
  slug: nothumansearch-ai-not-human-search-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-not-human-search-api-api-openapi.yml
- filename: nothumansearch-ai-provider-api-openapi.yml
  format: yaml
  label: Not Human Search Provider API
  slug: nothumansearch-ai-provider-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-provider-api-openapi.yml
- filename: nothumansearch-ai-quote-api-openapi.yml
  format: yaml
  label: Not Human Search Quote API
  slug: nothumansearch-ai-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-quote-api-openapi.yml
- filename: nothumansearch-ai-search-api-openapi.yml
  format: yaml
  label: Not Human Search Search API
  slug: nothumansearch-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-search-api-openapi.yml
- filename: nothumansearch-ai-site-api-openapi.yml
  format: yaml
  label: Not Human Search Site API
  slug: nothumansearch-ai-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-site-api-openapi.yml
- filename: nothumansearch-ai-stats-api-openapi.yml
  format: yaml
  label: Not Human Search Stats API
  slug: nothumansearch-ai-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-stats-api-openapi.yml
- filename: nothumansearch-ai-submit-api-openapi.yml
  format: yaml
  label: Not Human Search Submit API
  slug: nothumansearch-ai-submit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-submit-api-openapi.yml
- filename: nothumansearch-ai-top-api-openapi.yml
  format: yaml
  label: Not Human Search Top API
  slug: nothumansearch-ai-top-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-top-api-openapi.yml
- filename: nothumansearch-ai-verify-mcp-api-openapi.yml
  format: yaml
  label: Not Human Search Verify Mcp API
  slug: nothumansearch-ai-verify-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothumansearch-ai/openapi/nothumansearch-ai-verify-mcp-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Not Human Search Authentication
name_suffix: Authentication
oauth_flows: []
overview: Not Human Search secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Not Human Search
provider_slug: nothumansearch-ai
scheme_count: 2
schemes:
- description: Human account session created by the fail-closed email sign-in flow
  in: cookie
  name: SessionCookie
  parameter: nhs_session
  sources:
  - openapi/nothumansearch-ai-openapi.yaml
  type: apiKey
- description: Claim-scoped provider key returned once after DNS verification or explicit rotation; used for provider reads, acceptances, controlled-intent resolution, and outcome callbacks
  in: header
  name: ProviderKey
  parameter: X-NHS-Provider-Key
  sources:
  - openapi/nothumansearch-ai-openapi.yaml
  type: apiKey
slug: nothumansearch-ai-authentication
source_filename: nothumansearch-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nothumansearch-ai-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: SessionCookie\n  type: apiKey\n  in: cookie\n  parameter: nhs_session\n  description: Human account session created by the fail-closed email sign-in flow\n  sources:\n  - openapi/nothumansearch-ai-openapi.yaml\n- name: ProviderKey\n  type: apiKey\n  in: header\n  parameter: X-NHS-Provider-Key\n  description: Claim-scoped provider key returned once after DNS verification or explicit rotation;\n    used for provider reads, acceptances, controlled-intent resolution, and outcome callbacks\n  sources:\n  - openapi/nothumansearch-ai-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/nothumansearch-ai/authentication/nothumansearch-ai-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Artificial Intelligence
- Agent Readiness
- Search
- Analytics
---
