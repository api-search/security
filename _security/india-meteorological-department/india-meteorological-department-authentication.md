---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: India Meteorological Department Authentication
name_suffix: Authentication
oauth_flows: []
overview: India Meteorological Department declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: India Meteorological Department
provider_slug: india-meteorological-department
scheme_count: 1
schemes:
- description: The API requires a key. An unauthenticated GET to a documented endpoint returns HTTP 401 with the body {"error":"API key missing"}. The docs do not say which header or query parameter carries the key.
  evidence:
    observed_body: '{"error":"API key missing"}'
    observed_on: '2026-10-28'
    observed_status: 401
  in: unknown
  name: imd-api-key
  parameter_name: unknown
  portal_claims:
  - Secure JWT
  - Authenticated user onboarding with profile validation and controlled key-based API consumption.
  type: apiKey
slug: india-meteorological-department-authentication
source_filename: india-meteorological-department-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource:\n- https://api.imd.gov.in/public/index.php\n- https://api.imd.gov.in/api/v1/sunmoon?lat=26.9124&lon=75.7873\n- https://api.imd.gov.in/api/v1/current_wx\ndocs: https://api.imd.gov.in/public/index.php\nschemes:\n- name: imd-api-key\n  type: apiKey\n  in: unknown\n  parameter_name: unknown\n  description: The API requires a key. An unauthenticated GET to a documented endpoint returns HTTP 401 with the body\n    {\"error\":\"API key missing\"}. The docs do not say which header or query parameter carries the key.\n  evidence:\n    observed_status: 401\n    observed_body: '{\"error\":\"API key missing\"}'\n    observed_on: '2026-10-28'\n  portal_claims:\n  - 'Secure JWT'\n  - Authenticated user onboarding with profile validation and controlled key-based API consumption.\nsummary:\n  credential: API key issued after registering on the IMD API Management portal (https://api.imd.gov.in/public/register.php)\n    and logging in. The PDF\
  \ API document says organisations should contact the nodal officer and must follow IMD's terms and conditions.\n  note: The portal homepage mentions JWT, but the public API reference (api_reference.html) does not document the auth header,\n    the token format or how to obtain a JWT. Login and registration endpoints were not called.\n"
source_yaml_url: https://artifacts.apis.io/india-meteorological-department/authentication/india-meteorological-department-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Weather
- Meteorology
- India
- Public-Data
- Climate
- Government
---
