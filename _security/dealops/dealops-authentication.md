---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dealops-api-openapi-generated.yml
  format: yaml
  label: Dealops api API
  slug: api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealops/openapi/_ae-authored/dealops-api-openapi-generated.yml
- filename: dealops-core-openapi-generated.yml
  format: yaml
  label: Dealops core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealops/openapi/_ae-authored/dealops-core-openapi-generated.yml
auth_types: []
description: Authentication schemes for Dealops API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dealops Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dealops declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dealops
provider_slug: dealops
scheme_count: 1
schemes:
- evidence: 'Every request carries an organization API key in the x-api-key header:'
  header: x-api-key
  how_to_obtain: Keys are issued from Dealops settings by a user with API-key access. The key is displayed once, at creation; Dealops stores only an encrypted copy and cannot show it to you again.
  location: header
  name: x-api-key
  type: apiKey
slug: dealops-authentication
source_filename: dealops-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.dealops.com/docs/api/authentication/
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.dealops.com/docs/api/authentication/\nsources:\n- https://docs.dealops.com/docs/api/authentication/\n- https://docs.dealops.com/docs/category/getting-started/\n- https://docs.dealops.com/docs/getting-started/how-dealops-works/\n- https://docs.dealops.com/docs/getting-started/quote-lifecycle/\ndescription: Authentication schemes for Dealops API\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: 'Every request carries an organization API key in the x-api-key header:'\n  location: header\n  header: x-api-key\n  how_to_obtain: Keys are issued from Dealops settings by a user with API-key access. The key is displayed once, at creation; Dealops stores only\n    an encrypted copy and cannot show it to you again.\ndocs: https://docs.dealops.com/docs/api/authentication/\n"
source_yaml_url: https://artifacts.apis.io/dealops/authentication/dealops-authentication.yml
summary_line: 1 scheme
tags:
- Company
- CPQ
- Pricing
- Artificial Intelligence
- Software-as-a-Service
- Revenue-Optimization
---
