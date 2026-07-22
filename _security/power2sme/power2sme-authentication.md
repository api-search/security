---
api_key_in: []
api_specs:
- filename: power2sme-openapi.json
  format: json
  label: POWER2SME API
  slug: power2sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/power2sme/refs/heads/main/openapi/power2sme-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Power2Sme Authentication
name_suffix: Authentication
oauth_flows: []
overview: Power2SME declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Power2SME
provider_slug: power2sme
scheme_count: 0
schemes: []
slug: power2sme-authentication
source_filename: power2sme-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/power2sme-openapi.json (operations + 401/403 responses)\nprovider: power2sme\napi: POWER2SME API\nnotes: >-\n  The Swagger 2.0 document declares no `securityDefinitions`, so no formal\n  security scheme could be derived from the spec. Access is gated by a\n  login / OTP token model exposed through the operations themselves: callers\n  authenticate via the Sign In (customerloginUsingPOST) or OTP flow\n  (generateOtp* / validateOtp*) and every operation returns 401 Unauthorized\n  and 403 Forbidden, indicating a bearer/session token is expected on\n  subsequent calls. Token transport is not documented in the spec.\nschemes: []\nflows:\n- kind: login-token\n  evidence:\n  - operation: customerloginUsingPOST\n    path: /customerlogin\n    summary: Sign In\n  - operation: createPasswordUsingPOST\n    path: /createpassword\n    summary: Create New Password\n  - operation: changePasswordUsingPOST\n    path: /changepassword\n\
  \    summary: Change Password\n- kind: otp\n  evidence:\n  - operation: generateOtpUsingPOST_3\n    path: /generateotp\n    summary: Generate OTP\n  - operation: validateOtpUsingPOST_3\n    path: /validateotp\n    summary: Validate OTP\nunauthorized_responses:\n  '401': present on all 49 operations\n  '403': present on all 49 operations\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power2sme/refs/heads/main/authentication/power2sme-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Marketplaces
- SME
- Procurement
- India
- Onboarding
- OTP
- API
---
