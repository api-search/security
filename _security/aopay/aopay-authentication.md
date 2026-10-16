---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aopay-openapi-generated.yml
  format: yaml
  label: AOPAY Technology API
  slug: aopay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aopay/refs/heads/main/openapi/_ae-authored/aopay-openapi-generated.yml
auth_types: []
description: Authentication for AOPAY GST Verification API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aopay Authentication
name_suffix: Authentication
oauth_flows: []
overview: AOPAY Technology declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AOPAY Technology
provider_slug: aopay
scheme_count: 1
schemes:
- evidence: '-H "Authorization: Bearer YOUR_API_KEY"'
  header: Authorization
  how_to_obtain: Sign up for your API credentials
  location: header
  name: Bearer
  type: http-bearer
slug: aopay-authentication
source_filename: aopay-authentication.yml
source_heading: Authentication Profile
source_url: https://aopay.in/gst-verification-api
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://aopay.in/gst-verification-api\nsources:\n- https://aopay.in/gst-verification-api\ndescription: Authentication for AOPAY GST Verification API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '-H \"Authorization: Bearer YOUR_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up for your API credentials\ndocs: https://aopay.in/gst-verification-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aopay/refs/heads/main/authentication/aopay-authentication.yml
summary_line: 1 scheme
tags:
- Fintech
- Payments
- Banking
- NBFC
- API
---
