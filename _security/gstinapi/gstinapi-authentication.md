---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gstinapi-bulk-api-openapi.yml
  format: yaml
  label: GSTIN API Bulk API
  slug: gstinapi-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gstinapi/refs/heads/main/openapi/gstinapi-bulk-api-openapi.yml
- filename: gstinapi-verification-api-openapi.yml
  format: yaml
  label: GSTIN API Verification API
  slug: gstinapi-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gstinapi/refs/heads/main/openapi/gstinapi-verification-api-openapi.yml
auth_types: []
description: Authentication is a single header. The key identifies your account and meters your usage, so treat it as a credential rather than a configuration value.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Gstinapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: GSTIN API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GSTIN API
provider_slug: gstinapi
scheme_count: 1
schemes:
- evidence: Authentication is a single header. The key identifies your account and meters your usage, so treat it as a credential rather than a configuration value.
  header: x-api-key
  location: header
  name: API Key
  type: apiKey
slug: gstinapi-authentication
source_filename: gstinapi-authentication.yml
source_heading: Authentication Profile
source_url: https://gstinapi.com/blog/gst-api-integration-guide
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gstinapi.com/blog/gst-api-integration-guide\nsources:\n- https://gstinapi.com/blog/gst-api-integration-guide\n- https://gstinapi.com/blog/e-way-bill-2fa-authentication\n- https://gstinapi.com/blog/gst-aadhaar-authentication-registration\n- https://gstinapi.com/blog/gst-verification-vendor-onboarding\ndescription: Authentication is a single header. The key identifies your account and meters your usage, so treat it as a credential rather than\n  a configuration value.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Authentication is a single header. The key identifies your account and meters your usage, so treat it as a credential rather than\n    a configuration value.\n  location: header\n  header: x-api-key\ndocs: https://gstinapi.com/blog/gst-api-integration-guide\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gstinapi/refs/heads/main/authentication/gstinapi-authentication.yml
summary_line: 1 scheme
tags:
- Company
- GST
- India
- Taxation
- API
---
