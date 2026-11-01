---
anonymous_access: false
api_key_in: []
api_specs:
- filename: xpay-sh-rda-api-openapi.yml
  format: yaml
  label: xpay-sh Rda API
  slug: xpay-sh-rda-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpay-sh/openapi/xpay-sh-rda-api-openapi.yml
- filename: xpay-sh-rdas-api-openapi.yml
  format: yaml
  label: xpay-sh Rdas API
  slug: xpay-sh-rdas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpay-sh/openapi/xpay-sh-rdas-api-openapi.yml
- filename: xpay-sh-run-api-openapi.yml
  format: yaml
  label: xpay-sh Run API
  slug: xpay-sh-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpay-sh/openapi/xpay-sh-run-api-openapi.yml
- filename: xpay-sh-wallet-api-openapi.yml
  format: yaml
  label: xpay-sh Wallet API
  slug: xpay-sh-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/xpay-sh/openapi/xpay-sh-wallet-api-openapi.yml
auth_types: []
description: Authentication uses an API key that is sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Xpay Sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: xpay-sh declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: xpay-sh
provider_slug: xpay-sh
scheme_count: 1
schemes:
- evidence: 'Your key will look like: xpay_sk_... Copy it — you’ll need it in the next step.'
  header: Authorization
  how_to_obtain: Create an API key in the xpay account UI (Account → API Keys) and copy the generated key.
  location: header
  name: API Key
  type: http-bearer
slug: xpay-sh-authentication
source_filename: xpay-sh-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.xpay.sh/en/merchants/woocommerce/rest-api-keys
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.xpay.sh/en/merchants/woocommerce/rest-api-keys\nsources:\n- https://docs.xpay.sh/en/merchants/woocommerce/rest-api-keys\n- https://docs.xpay.sh/en/tools/get-started/get-api-key\n- https://docs.xpay.sh/en/getting-started\n- https://docs.xpay.sh/en/getting-started/installation\ndescription: Authentication uses an API key that is sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Your key will look like: xpay_sk_... Copy it — you’ll need it in the next step.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the xpay account UI (Account → API Keys) and copy the generated key.\ndocs: https://docs.xpay.sh/en/merchants/woocommerce/rest-api-keys\n"
source_yaml_url: https://artifacts.apis.io/xpay-sh/authentication/xpay-sh-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Commerce
- AI
- SaaS
- AgentReadiness
---
