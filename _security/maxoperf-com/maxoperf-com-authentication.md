---
anonymous_access: false
api_key_in: []
api_specs:
- filename: maxoperf-com-academy-openapi-generated.yml
  format: yaml
  label: MaxoPerf Overview API
  slug: academy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxoperf-com/openapi/_ae-authored/maxoperf-com-academy-openapi-generated.yml
- filename: maxoperf-com-core-openapi-generated.yml
  format: yaml
  label: MaxoPerf core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxoperf-com/openapi/_ae-authored/maxoperf-com-core-openapi-generated.yml
- filename: maxoperf-com-dependencies-openapi-generated.yml
  format: yaml
  label: MaxoPerf Overview API
  slug: dependencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxoperf-com/openapi/_ae-authored/maxoperf-com-dependencies-openapi-generated.yml
- filename: maxoperf-com-how-to-openapi-generated.yml
  format: yaml
  label: MaxoPerf how to API
  slug: how-to-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maxoperf-com/openapi/_ae-authored/maxoperf-com-how-to-openapi-generated.yml
auth_types: []
description: Authentication methods for MaxoPerf API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MaxoPerf Authentication
name_suffix: Authentication
oauth_flows: []
overview: MaxoPerf declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MaxoPerf
provider_slug: maxoperf-com
scheme_count: 1
schemes:
- evidence: 'Pass the key as a bearer token:'
  header: Authorization
  how_to_obtain: Create a new API key in Settings → API keys, copy the token shown (mpak_<keyId>_<secret>)
  location: header
  name: API key
  type: http-bearer
slug: maxoperf-com-authentication
source_filename: maxoperf-com-authentication.yml
source_heading: Authentication Profile
source_url: https://maxoperf.com/docs/how-to/get-an-api-key
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://maxoperf.com/docs/how-to/get-an-api-key\nsources:\n- https://maxoperf.com/docs/how-to/get-an-api-key\n- https://maxoperf.com/docs/academy/cookbook/auth-login-token-flow\n- https://maxoperf.com/docs/academy/ai-testing/streaming-and-token-latency-testing\n- https://maxoperf.com/docs/academy/ai-testing/inference-cost-and-token-budget-testing\ndescription: Authentication methods for MaxoPerf API\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Pass the key as a bearer token:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a new API key in Settings → API keys, copy the token shown (mpak_<keyId>_<secret>)\ndocs: https://maxoperf.com/docs/how-to/get-an-api-key\n"
source_yaml_url: https://artifacts.apis.io/maxoperf-com/authentication/maxoperf-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Performance Testing
- Load Testing
- Cloud
---
