---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ip1sms-openapi-generated.yml
  format: yaml
  label: iP1 SMS API
  slug: ip1sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ip1sms/openapi/_ae-authored/ip1sms-openapi-generated.yml
auth_types: []
description: Authentication is performed by sending an HTTP Authorization header with the scheme "Bearer" followed by the API Key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: iP1 SMS Authentication
name_suffix: Authentication
oauth_flows: []
overview: iP1 SMS declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: iP1 SMS
provider_slug: ip1sms
scheme_count: 1
schemes:
- evidence: client.DefaultRequestHeaders.Authorization = new AuthenticationHeaderValue("Bearer", "API Key");
  header: Authorization
  how_to_obtain: Create a free developer account on iP1 SMS and retrieve your API Key from the user portal.
  location: header
  name: Bearer
  type: http-bearer
slug: ip1sms-authentication
source_filename: ip1sms-authentication.yml
source_heading: Authentication Profile
source_url: https://ip1sms.com/en/multi-factor-authentication-via-sms/
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ip1sms.com/en/multi-factor-authentication-via-sms/\nsources:\n- https://ip1sms.com/en/multi-factor-authentication-via-sms/\ndescription: Authentication is performed by sending an HTTP Authorization header with the scheme \"Bearer\" followed by the API Key.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: client.DefaultRequestHeaders.Authorization = new AuthenticationHeaderValue(\"Bearer\", \"API Key\");\n  location: header\n  header: Authorization\n  how_to_obtain: Create a free developer account on iP1 SMS and retrieve your API Key from the user portal.\ndocs: https://ip1sms.com/en/multi-factor-authentication-via-sms/\n"
source_yaml_url: https://artifacts.apis.io/ip1sms/authentication/ip1sms-authentication.yml
summary_line: 1 scheme
tags:
- Company
- SMS
- Communications
- Enterprise
- Integration
---
