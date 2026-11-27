---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ffraud-com-account-api-openapi.yml
  format: yaml
  label: FFraud Account API
  slug: ffraud-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-account-api-openapi.yml
- filename: ffraud-com-community-api-openapi.yml
  format: yaml
  label: FFraud Community API
  slug: ffraud-com-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-community-api-openapi.yml
- filename: ffraud-com-compatibility-api-openapi.yml
  format: yaml
  label: FFraud Compatibility API
  slug: ffraud-com-compatibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-compatibility-api-openapi.yml
- filename: ffraud-com-device-api-openapi.yml
  format: yaml
  label: FFraud Device API
  slug: ffraud-com-device-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-device-api-openapi.yml
- filename: ffraud-com-domain-api-openapi.yml
  format: yaml
  label: FFraud Domain API
  slug: ffraud-com-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-domain-api-openapi.yml
- filename: ffraud-com-email-api-openapi.yml
  format: yaml
  label: FFraud Email API
  slug: ffraud-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-email-api-openapi.yml
- filename: ffraud-com-ip-api-openapi.yml
  format: yaml
  label: FFraud IP API
  slug: ffraud-com-ip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-ip-api-openapi.yml
- filename: ffraud-com-system-api-openapi.yml
  format: yaml
  label: FFraud System API
  slug: ffraud-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ffraud-com/openapi/ffraud-com-system-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: FFraud Authentication
name_suffix: Authentication
oauth_flows: []
overview: FFraud declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FFraud
provider_slug: ffraud-com
scheme_count: 1
schemes:
- evidence: 'Pass your key in the X-API-Key header:'
  header: X-API-Key
  how_to_obtain: Create a free account and your key is shown once, immediately.
  location: header
  name: X-API-Key
  type: apiKey
slug: ffraud-com-authentication
source_filename: ffraud-com-authentication.yml
source_heading: Authentication Profile
source_url: https://ffraud.com/docs/authentication
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ffraud.com/docs/authentication\nsources:\n- https://ffraud.com/docs/authentication\n- https://ffraud.com/blog/block-disposable-emails-supabase\n- https://ffraud.com/blog/block-disposable-emails-nextjs-express\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Pass your key in the X-API-Key header:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a free account and your key is shown once, immediately.\nnote: Public /public/* endpoints require no authentication.\ndocs: https://ffraud.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/ffraud-com/authentication/ffraud-com-authentication.yml
summary_line: 1 scheme
tags:
- Fraud Prevention
- IP Lookup
- Email Verification
- Device Fingerprinting
- Open Data
---
