---
anonymous_access: false
api_key_in: []
api_specs:
- filename: moneygraph-ai-openapi-generated.yml
  format: yaml
  label: MoneyGraph.AI API
  slug: moneygraph-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moneygraph-ai/openapi/_ae-authored/moneygraph-ai-openapi-generated.yml
auth_types: []
description: Every API request is signed with your API secret using HMAC-SHA256 and carries a unique nonce and Idempotency-Key. There are no bearer tokens to exchange or refresh.
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: MoneyGraph.AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: MoneyGraph.AI declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: MoneyGraph.AI
provider_slug: moneygraph-ai
scheme_count: 5
schemes:
- evidence: Every API request is signed with your API secret using HMAC-SHA256 and carries a unique nonce and Idempotency-Key.
  header: X-Key-Id
  how_to_obtain: Create API keys in your dashboard under Developers, API keys.
  location: header
  name: MoneyGraph HMAC
  type: hmac
- evidence: Send these headers with every request to https://app.moneygraph.ai/api/v1 .
  header: X-Timestamp
  location: header
  name: MoneyGraph HMAC Timestamp
  type: hmac
- evidence: Send these headers with every request to https://app.moneygraph.ai/api/v1 .
  header: X-Nonce
  location: header
  name: MoneyGraph HMAC Nonce
  type: hmac
- evidence: Send these headers with every request to https://app.moneygraph.ai/api/v1 .
  header: X-Signature
  location: header
  name: MoneyGraph HMAC Signature
  type: hmac
- evidence: A unique value for every request, at most 50 characters. It is not part of the signature.
  header: Idempotency-Key
  location: header
  name: Idempotency-Key
  type: other
slug: moneygraph-ai-authentication
source_filename: moneygraph-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://app.moneygraph.ai/docs/guide/authentication
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://app.moneygraph.ai/docs/guide/authentication\nsources:\n- https://app.moneygraph.ai/docs/guide/authentication\n- https://app.moneygraph.ai/docs/reference/customers/mfa-setup\n- https://app.moneygraph.ai/docs/guide/onboarding\ndescription: Every API request is signed with your API secret using HMAC-SHA256 and carries a unique nonce and Idempotency-Key. There are no bearer\n  tokens to exchange or refresh.\nschemes:\n- type: hmac\n  name: MoneyGraph HMAC\n  evidence: Every API request is signed with your API secret using HMAC-SHA256 and carries a unique nonce and Idempotency-Key.\n  location: header\n  header: X-Key-Id\n  how_to_obtain: Create API keys in your dashboard under Developers, API keys.\n- type: hmac\n  name: MoneyGraph HMAC Timestamp\n  evidence: Send these headers with every request to https://app.moneygraph.ai/api/v1 .\n  location: header\n  header: X-Timestamp\n\
  - type: hmac\n  name: MoneyGraph HMAC Nonce\n  evidence: Send these headers with every request to https://app.moneygraph.ai/api/v1 .\n  location: header\n  header: X-Nonce\n- type: hmac\n  name: MoneyGraph HMAC Signature\n  evidence: Send these headers with every request to https://app.moneygraph.ai/api/v1 .\n  location: header\n  header: X-Signature\n- type: other\n  name: Idempotency-Key\n  evidence: A unique value for every request, at most 50 characters. It is not part of the signature.\n  location: header\n  header: Idempotency-Key\nnote: Only HMAC‑based authentication is documented; no OAuth2 flows, bearer tokens, or other schemes are mentioned.\ndocs: https://app.moneygraph.ai/docs/guide/authentication\n"
source_yaml_url: https://artifacts.apis.io/moneygraph-ai/authentication/moneygraph-ai-authentication.yml
summary_line: 5 schemes
tags:
- Fintech
- Payments
- Artificial Intelligence
- SDK
- Global
---
