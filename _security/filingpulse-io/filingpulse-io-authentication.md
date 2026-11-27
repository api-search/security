---
anonymous_access: false
api_key_in: []
api_specs:
- filename: filingpulse-io-account-api-openapi.yml
  format: yaml
  label: FilingPulse Account API
  slug: filingpulse-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingpulse-io/openapi/filingpulse-io-account-api-openapi.yml
- filename: filingpulse-io-events-api-openapi.yml
  format: yaml
  label: FilingPulse Events API
  slug: filingpulse-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingpulse-io/openapi/filingpulse-io-events-api-openapi.yml
- filename: filingpulse-io-filings-api-openapi.yml
  format: yaml
  label: FilingPulse Filings API
  slug: filingpulse-io-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingpulse-io/openapi/filingpulse-io-filings-api-openapi.yml
- filename: filingpulse-io-meta-api-openapi.yml
  format: yaml
  label: FilingPulse Meta API
  slug: filingpulse-io-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingpulse-io/openapi/filingpulse-io-meta-api-openapi.yml
- filename: filingpulse-io-registrations-api-openapi.yml
  format: yaml
  label: FilingPulse Registrations API
  slug: filingpulse-io-registrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingpulse-io/openapi/filingpulse-io-registrations-api-openapi.yml
- filename: filingpulse-io-signup-api-openapi.yml
  format: yaml
  label: FilingPulse Signup API
  slug: filingpulse-io-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingpulse-io/openapi/filingpulse-io-signup-api-openapi.yml
- filename: filingpulse-io-webhooks-api-openapi.yml
  format: yaml
  label: FilingPulse Webhooks API
  slug: filingpulse-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filingpulse-io/openapi/filingpulse-io-webhooks-api-openapi.yml
auth_types: []
description: FilingPulse uses an API key that is emailed to the user and works immediately.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FilingPulse Authentication
name_suffix: Authentication
oauth_flows: []
overview: FilingPulse declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FilingPulse
provider_slug: filingpulse-io
scheme_count: 1
schemes:
- evidence: The key is emailed to you and works immediately.
  how_to_obtain: The key is emailed to you after signing up (free tier) or after secure checkout via Stripe (paid tiers).
  name: API Key
  type: apiKey
slug: filingpulse-io-authentication
source_filename: filingpulse-io-authentication.yml
source_heading: Authentication Profile
source_url: https://filingpulse.io/signup.html
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://filingpulse.io/signup.html\nsources:\n- https://filingpulse.io/signup.html\ndescription: FilingPulse uses an API key that is emailed to the user and works immediately.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: The key is emailed to you and works immediately.\n  how_to_obtain: The key is emailed to you after signing up (free tier) or after secure checkout via Stripe (paid tiers).\ndocs: https://filingpulse.io/signup.html\n"
source_yaml_url: https://artifacts.apis.io/filingpulse-io/authentication/filingpulse-io-authentication.yml
summary_line: 1 scheme
tags:
- SEC EDGAR
- Regulatory Filings
- Insider Trading
- Form 4
- 8-K
- S-1 / IPO Registrations
- Financial Data
- Webhook
- REST API
- MCP Server
---
