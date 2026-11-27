---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: maginary-ai-api-keys-api-openapi.yml
  format: yaml
  label: Maginary API Keys API
  slug: maginary-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maginary-ai/openapi/maginary-ai-api-keys-api-openapi.yml
- filename: maginary-ai-auth-api-openapi.yml
  format: yaml
  label: Maginary Auth API
  slug: maginary-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maginary-ai/openapi/maginary-ai-auth-api-openapi.yml
- filename: maginary-ai-checkout-stripe-api-openapi.yml
  format: yaml
  label: Maginary Checkout Stripe API
  slug: maginary-ai-checkout-stripe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maginary-ai/openapi/maginary-ai-checkout-stripe-api-openapi.yml
- filename: maginary-ai-credit-check-api-openapi.yml
  format: yaml
  label: Maginary Credit Check API
  slug: maginary-ai-credit-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maginary-ai/openapi/maginary-ai-credit-check-api-openapi.yml
- filename: maginary-ai-credits-config-api-openapi.yml
  format: yaml
  label: Maginary Credits Config API
  slug: maginary-ai-credits-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maginary-ai/openapi/maginary-ai-credits-config-api-openapi.yml
- filename: maginary-ai-events-api-openapi.yml
  format: yaml
  label: Maginary Events API
  slug: maginary-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maginary-ai/openapi/maginary-ai-events-api-openapi.yml
- filename: maginary-ai-faqs-api-openapi.yml
  format: yaml
  label: Maginary Faqs API
  slug: maginary-ai-faqs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maginary-ai/openapi/maginary-ai-faqs-api-openapi.yml
- filename: maginary-ai-gens-api-openapi.yml
  format: yaml
  label: Maginary Gens API
  slug: maginary-ai-gens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maginary-ai/openapi/maginary-ai-gens-api-openapi.yml
- filename: maginary-ai-image-of-the-day-api-openapi.yml
  format: yaml
  label: Maginary Image Of The Day API
  slug: maginary-ai-image-of-the-day-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maginary-ai/openapi/maginary-ai-image-of-the-day-api-openapi.yml
- filename: maginary-ai-products-api-openapi.yml
  format: yaml
  label: Maginary Products API
  slug: maginary-ai-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maginary-ai/openapi/maginary-ai-products-api-openapi.yml
- filename: maginary-ai-profiles-api-openapi.yml
  format: yaml
  label: Maginary Profiles API
  slug: maginary-ai-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maginary-ai/openapi/maginary-ai-profiles-api-openapi.yml
- filename: maginary-ai-public-api-openapi.yml
  format: yaml
  label: Maginary Public API
  slug: maginary-ai-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maginary-ai/openapi/maginary-ai-public-api-openapi.yml
- filename: maginary-ai-recipes-api-openapi.yml
  format: yaml
  label: Maginary Recipes API
  slug: maginary-ai-recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maginary-ai/openapi/maginary-ai-recipes-api-openapi.yml
- filename: maginary-ai-reviews-api-openapi.yml
  format: yaml
  label: Maginary Reviews API
  slug: maginary-ai-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maginary-ai/openapi/maginary-ai-reviews-api-openapi.yml
- filename: maginary-ai-seo-api-openapi.yml
  format: yaml
  label: Maginary Seo API
  slug: maginary-ai-seo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maginary-ai/openapi/maginary-ai-seo-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Maginary Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maginary secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Maginary
provider_slug: maginary-ai
scheme_count: 2
schemes:
- name: Basic
  scheme: basic
  sources:
  - openapi/maginary-ai-openapi.yml
  type: http
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/maginary-ai-openapi.yml
  type: apiKey
slug: maginary-ai-authentication
source_filename: maginary-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/maginary-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/maginary-ai-openapi.yml\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/maginary-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/maginary-ai/authentication/maginary-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI Generation
- Image Generation
- Video Generation
- Creative Tools
---
