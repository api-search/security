---
anonymous_access: false
api_key_in: []
api_specs:
- filename: horsetruth-openapi-generated.yml
  format: yaml
  label: Horse Truth API
  slug: horsetruth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/horsetruth/refs/heads/main/openapi/_ae-authored/horsetruth-openapi-generated.yml
auth_types: []
description: Authentication schemes for Horse Truth API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Horsetruth Authentication
name_suffix: Authentication
oauth_flows: []
overview: Horse Truth declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Horse Truth
provider_slug: horsetruth
scheme_count: 1
schemes:
- evidence: With x402 the first reply is HTTP 402 with a PAYMENT-REQUIRED header (base64 JSON). Sign it, send PAYMENT-SIGNATURE , and retry the same request.
  header: PAYMENT-SIGNATURE
  location: header
  name: x402 payment signature
  type: other
slug: horsetruth-authentication
source_filename: horsetruth-authentication.yml
source_heading: Authentication Profile
source_url: https://horsetruth.com.au/developers/machine
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://horsetruth.com.au/developers/machine\nsources:\n- https://horsetruth.com.au/developers/machine\ndescription: Authentication schemes for Horse Truth API\nschemes:\n- type: other\n  name: x402 payment signature\n  evidence: With x402 the first reply is HTTP 402 with a PAYMENT-REQUIRED header (base64 JSON). Sign it, send PAYMENT-SIGNATURE , and retry the\n    same request.\n  location: header\n  header: PAYMENT-SIGNATURE\ndocs: https://horsetruth.com.au/developers/machine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horsetruth/refs/heads/main/authentication/horsetruth-authentication.yml
summary_line: 1 scheme
tags:
- Racehorse Intelligence
- Horse Reports
- API
- Developers
- Trainers
---
