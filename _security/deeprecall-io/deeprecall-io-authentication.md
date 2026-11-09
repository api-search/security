---
anonymous_access: false
api_key_in: []
api_specs:
- filename: deeprecall-io-health-api-openapi.yml
  format: yaml
  label: DeepRecall Health API
  slug: deeprecall-io-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deeprecall-io/openapi/deeprecall-io-health-api-openapi.yml
- filename: deeprecall-io-recalls-api-openapi.yml
  format: yaml
  label: DeepRecall Recalls API
  slug: deeprecall-io-recalls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deeprecall-io/openapi/deeprecall-io-recalls-api-openapi.yml
auth_types: []
description: DeepRecall API uses API key authentication for all requests (except the public /health endpoint).
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Deeprecall Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeepRecall declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DeepRecall
provider_slug: deeprecall-io
scheme_count: 1
schemes:
- evidence: 'Include your API key in the X-API-Key header with every request:'
  header: X-API-Key
  how_to_obtain: Request access via email, receive your API key via secure email.
  location: header
  name: API Key
  type: apiKey
slug: deeprecall-io-authentication
source_filename: deeprecall-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.deeprecall.io/authentication
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.deeprecall.io/authentication\nsources:\n- https://docs.deeprecall.io/authentication\n- https://docs.deeprecall.io/quickstart\ndescription: DeepRecall API uses API key authentication for all requests (except the public /health endpoint).\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Include your API key in the X-API-Key header with every request:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Request access via email, receive your API key via secure email.\nnote: No OAuth2 or other authentication schemes are documented.\ndocs: https://docs.deeprecall.io/authentication\n"
source_yaml_url: https://artifacts.apis.io/deeprecall-io/authentication/deeprecall-io-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Regulatory
- Marketplace
- Compliance
- Intelligence
---
