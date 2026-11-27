---
anonymous_access: false
api_key_in: []
api_specs:
- filename: docimprint-com-billing-api-openapi.yml
  format: yaml
  label: DocImprint Billing API
  slug: docimprint-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-billing-api-openapi.yml
- filename: docimprint-com-check-claims-api-openapi.yml
  format: yaml
  label: DocImprint Check Claims API
  slug: docimprint-com-check-claims-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-check-claims-api-openapi.yml
- filename: docimprint-com-checkpoints-api-openapi.yml
  format: yaml
  label: DocImprint Checkpoints API
  slug: docimprint-com-checkpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-checkpoints-api-openapi.yml
- filename: docimprint-com-collections-api-openapi.yml
  format: yaml
  label: DocImprint Collections API
  slug: docimprint-com-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-collections-api-openapi.yml
- filename: docimprint-com-describe-api-openapi.yml
  format: yaml
  label: DocImprint Describe API
  slug: docimprint-com-describe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-describe-api-openapi.yml
- filename: docimprint-com-extract-api-openapi.yml
  format: yaml
  label: DocImprint Extract API
  slug: docimprint-com-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-extract-api-openapi.yml
- filename: docimprint-com-feedback-api-openapi.yml
  format: yaml
  label: DocImprint Feedback API
  slug: docimprint-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-feedback-api-openapi.yml
- filename: docimprint-com-jobs-api-openapi.yml
  format: yaml
  label: DocImprint Jobs API
  slug: docimprint-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-jobs-api-openapi.yml
- filename: docimprint-com-keys-api-openapi.yml
  format: yaml
  label: DocImprint Keys API
  slug: docimprint-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-keys-api-openapi.yml
- filename: docimprint-com-monitor-api-openapi.yml
  format: yaml
  label: DocImprint Monitor API
  slug: docimprint-com-monitor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-monitor-api-openapi.yml
- filename: docimprint-com-qa-api-openapi.yml
  format: yaml
  label: DocImprint Qa API
  slug: docimprint-com-qa-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-qa-api-openapi.yml
- filename: docimprint-com-quickstart-api-openapi.yml
  format: yaml
  label: DocImprint Quickstart API
  slug: docimprint-com-quickstart-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-quickstart-api-openapi.yml
- filename: docimprint-com-quota-api-openapi.yml
  format: yaml
  label: DocImprint Quota API
  slug: docimprint-com-quota-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-quota-api-openapi.yml
- filename: docimprint-com-summarize-api-openapi.yml
  format: yaml
  label: DocImprint Summarize API
  slug: docimprint-com-summarize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-summarize-api-openapi.yml
- filename: docimprint-com-translate-api-openapi.yml
  format: yaml
  label: DocImprint Translate API
  slug: docimprint-com-translate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docimprint-com/openapi/docimprint-com-translate-api-openapi.yml
auth_types: []
description: 'DocImprint supports two authentication schemes: API keys and x402 USDC micropayments.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: DocImprint Authentication
name_suffix: Authentication
oauth_flows: []
overview: DocImprint declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DocImprint
provider_slug: docimprint-com
scheme_count: 2
schemes:
- evidence: 'API keys: send Authorization: Bearer dr_live_.... The API key is tied to a Stripe subscription plan with monthly credits.'
  header: Authorization
  how_to_obtain: Get an API key from the dashboard (Free monthly credits or paid plan).
  location: header
  name: API key
  type: http-bearer
- evidence: 'x402: send no auth header. The server responds with 402 and payment requirements. Sign a USDC transfer on Base and retry.'
  header: X-Payment
  how_to_obtain: Sign an EIP‑712 USDC transfer for the amount indicated in the 402 response and include it in the X-Payment header.
  location: header
  name: x402
  type: other
slug: docimprint-com-authentication
source_filename: docimprint-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docimprint.com/blog/x402-vs-api-keys
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docimprint.com/blog/x402-vs-api-keys\nsources:\n- https://docimprint.com/blog/x402-vs-api-keys\n- https://docimprint.com/docs/authentication\n- https://docimprint.com/docs/getting-started\n- https://docimprint.com/docs/agents\ndescription: 'DocImprint supports two authentication schemes: API keys and x402 USDC micropayments.'\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'API keys: send Authorization: Bearer dr_live_.... The API key is tied to a Stripe subscription plan with monthly credits.'\n  location: header\n  header: Authorization\n  how_to_obtain: Get an API key from the dashboard (Free monthly credits or paid plan).\n- type: other\n  name: x402\n  evidence: 'x402: send no auth header. The server responds with 402 and payment requirements. Sign a USDC transfer on Base and retry.'\n  location: header\n  header: X-Payment\n  how_to_obtain: Sign an EIP‑712\
  \ USDC transfer for the amount indicated in the 402 response and include it in the X-Payment header.\nnote: No OAuth2 flows are documented for DocImprint.\ndocs: https://docimprint.com/blog/x402-vs-api-keys\n"
source_yaml_url: https://artifacts.apis.io/docimprint-com/authentication/docimprint-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Documents
- Verification
- Cryptography
- Payments
- Company
---
