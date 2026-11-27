---
anonymous_access: false
api_key_in: []
api_specs:
- filename: icme-io-checkitpaid-api-openapi.yml
  format: yaml
  label: ICME Labs Check It Paid API
  slug: icme-io-checkitpaid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/icme-io/openapi/icme-io-checkitpaid-api-openapi.yml
- filename: icme-io-createuserx402-api-openapi.yml
  format: yaml
  label: ICME Labs Create User X402 API
  slug: icme-io-createuserx402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/icme-io/openapi/icme-io-createuserx402-api-openapi.yml
- filename: icme-io-topupx402-api-openapi.yml
  format: yaml
  label: ICME Labs Top Up X402 API
  slug: icme-io-topupx402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/icme-io/openapi/icme-io-topupx402-api-openapi.yml
auth_types: []
description: Authentication for ICME Labs API uses an API key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ICME Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: ICME Labs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ICME Labs
provider_slug: icme-io
scheme_count: 1
schemes:
- evidence: You'll receive your `api_key`. Save it — you'll need it for every authenticated request.
  header: X-API-Key
  how_to_obtain: Create an account (pay $5 via card or USDC), then retrieve the API key from the checkout URL or via the `/v1/session/SESSION_ID` endpoint.
  location: header
  name: API Key
  type: apiKey
slug: icme-io-authentication
source_filename: icme-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.icme.io/documentation/getting-started/quickstart.md
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.icme.io/documentation/getting-started/quickstart.md\nsources:\n- https://docs.icme.io/documentation/getting-started/quickstart.md\n- https://docs.icme.io/documentation/getting-started/pricing.md\n- https://docs.icme.io/documentation/getting-started/stop-watching-your-agents.-start-proving-theyre-right..md\ndescription: Authentication for ICME Labs API uses an API key.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: You'll receive your `api_key`. Save it — you'll need it for every authenticated request.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an account (pay $5 via card or USDC), then retrieve the API key from the checkout URL or via the `/v1/session/SESSION_ID`\n    endpoint.\ndocs: https://docs.icme.io/documentation/getting-started/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/icme-io/authentication/icme-io-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Verification
- Compliance
- Enterprise
- Security
- Company
---
