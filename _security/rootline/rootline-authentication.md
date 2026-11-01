---
anonymous_access: false
api_key_in: []
api_specs:
- filename: rootline-core-openapi-generated.yml
  format: yaml
  label: Rootline core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rootline/openapi/_ae-authored/rootline-core-openapi-generated.yml
- filename: rootline-in-person-payments-openapi-generated.yml
  format: yaml
  label: Rootline in person payments API
  slug: in-person-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rootline/openapi/_ae-authored/rootline-in-person-payments-openapi-generated.yml
- filename: rootline-payments-openapi-generated.yml
  format: yaml
  label: Rootline payments API
  slug: payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rootline/openapi/_ae-authored/rootline-payments-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Rootline Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rootline declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Rootline
provider_slug: rootline
scheme_count: 1
schemes:
- description: API key provided in x-api-key header. Starts with sk_rootline_.
  in: header
  name: x-api-key
  type: apiKey
slug: rootline-authentication
source_filename: rootline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://docs.rootline.com/guides/get-started/api-keys\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: \"API key provided in x-api-key header. Starts with sk_rootline_.\"\n"
source_yaml_url: https://artifacts.apis.io/rootline/authentication/rootline-authentication.yml
summary_line: 1 scheme
tags:
- Payments
- FinTech
- EmbeddedPayments
- API
- Platform
---
