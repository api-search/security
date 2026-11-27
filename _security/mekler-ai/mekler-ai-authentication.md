---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: mekler-ai-api-monitoring-api-openapi.yml
  format: yaml
  label: Mekler AI API monitoring API
  slug: mekler-ai-api-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-api-monitoring-api-openapi.yml
- filename: mekler-ai-compute-api-openapi.yml
  format: yaml
  label: Mekler AI Compute API
  slug: mekler-ai-compute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-compute-api-openapi.yml
- filename: mekler-ai-csv-api-openapi.yml
  format: yaml
  label: Mekler AI CSV API
  slug: mekler-ai-csv-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-csv-api-openapi.yml
- filename: mekler-ai-data-api-openapi.yml
  format: yaml
  label: Mekler AI Data API
  slug: mekler-ai-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-data-api-openapi.yml
- filename: mekler-ai-directory-api-openapi.yml
  format: yaml
  label: Mekler AI Directory API
  slug: mekler-ai-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-directory-api-openapi.yml
- filename: mekler-ai-email-api-openapi.yml
  format: yaml
  label: Mekler AI Email API
  slug: mekler-ai-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-email-api-openapi.yml
- filename: mekler-ai-finance-api-openapi.yml
  format: yaml
  label: Mekler AI Finance API
  slug: mekler-ai-finance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-finance-api-openapi.yml
- filename: mekler-ai-images-api-openapi.yml
  format: yaml
  label: Mekler AI Images API
  slug: mekler-ai-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-images-api-openapi.yml
- filename: mekler-ai-inference-api-openapi.yml
  format: yaml
  label: Mekler AI Inference API
  slug: mekler-ai-inference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-inference-api-openapi.yml
- filename: mekler-ai-listing-monitoring-api-openapi.yml
  format: yaml
  label: Mekler AI listing monitoring API
  slug: mekler-ai-listing-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-listing-monitoring-api-openapi.yml
- filename: mekler-ai-messaging-api-openapi.yml
  format: yaml
  label: Mekler AI Messaging API
  slug: mekler-ai-messaging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-messaging-api-openapi.yml
- filename: mekler-ai-news-api-openapi.yml
  format: yaml
  label: Mekler AI News API
  slug: mekler-ai-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-news-api-openapi.yml
- filename: mekler-ai-research-api-openapi.yml
  format: yaml
  label: Mekler AI Research API
  slug: mekler-ai-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-research-api-openapi.yml
- filename: mekler-ai-sanctions-api-openapi.yml
  format: yaml
  label: Mekler AI Sanctions API
  slug: mekler-ai-sanctions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-sanctions-api-openapi.yml
- filename: mekler-ai-services-api-openapi.yml
  format: yaml
  label: Mekler AI Services API
  slug: mekler-ai-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-services-api-openapi.yml
- filename: mekler-ai-web-api-openapi.yml
  format: yaml
  label: Mekler AI Web API
  slug: mekler-ai-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-web-api-openapi.yml
- filename: mekler-ai-x402-api-openapi.yml
  format: yaml
  label: Mekler AI X402 API
  slug: mekler-ai-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mekler-ai/openapi/mekler-ai-x402-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Mekler AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mekler AI secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mekler AI
provider_slug: mekler-ai
scheme_count: 3
schemes:
- description: x402 v2 payment, not an account credential. An unsigned POST returns 402 with PAYMENT-REQUIRED; sign one accepts[] offer and resend the same request with PAYMENT-SIGNATURE. No API key or signup.
  name: x402
  scheme: x402
  sources:
  - openapi/mekler-ai-openapi.json
  - openapi/openapi.json
  type: http
- description: Caller-generated private access_key for this inbox; no account/API key registration. Free read/delete operations only.
  name: inboxCapability
  scheme: bearer
  sources:
  - openapi/mekler-ai-openapi.json
  - openapi/openapi.json
  type: http
- description: Private domain-control capability, unrelated to payment.
  in: header
  name: listingControl
  parameter: X-Mekler-Listing-Control
  sources:
  - openapi/mekler-ai-openapi.json
  - openapi/openapi.json
  type: apiKey
slug: mekler-ai-authentication
source_filename: mekler-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/mekler-ai-openapi.json, openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: x402\n  type: http\n  scheme: x402\n  description: x402 v2 payment, not an account credential. An unsigned POST returns 402 with\n    PAYMENT-REQUIRED; sign one accepts[] offer and resend the same request with PAYMENT-SIGNATURE.\n    No API key or signup.\n  sources:\n  - openapi/mekler-ai-openapi.json\n  - openapi/openapi.json\n- name: inboxCapability\n  type: http\n  scheme: bearer\n  description: Caller-generated private access_key for this inbox; no account/API key registration.\n    Free read/delete operations only.\n  sources:\n  - openapi/mekler-ai-openapi.json\n  - openapi/openapi.json\n- name: listingControl\n  type: apiKey\n  in: header\n  parameter: X-Mekler-Listing-Control\n  description: Private domain-control capability, unrelated to payment.\n  sources:\n  - openapi/mekler-ai-openapi.json\n\
  \  - openapi/openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mekler-ai/authentication/mekler-ai-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Artificial Intelligence
- Assistant
- Services
- Automation
---
