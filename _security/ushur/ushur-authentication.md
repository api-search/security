---
api_key_in: []
auth_types:
- session-login
- otp
description: ''
kind: authentication
layout: security
method: searched
name: Ushur Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ushur secures its APIs with session-login and otp across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ushur
provider_slug: ushur
scheme_count: 2
schemes:
- description: Email + password login against the tenant API host (for example https://apidev.ushur.me/ in SDK examples; production tenants use their own *.ushur.me host). Emits loginSuccess/loginFailure; all subsequent SDK calls reuse the authenticated session.
  name: platform-login
  sources:
  - https://github.com/UshurInc/UshurNodeSDK#usage
  type: session
- description: Two-step end-user verification. ushur.authentication({phoneNumber}) triggers an OTP and returns a phAuthTransactionId; ushur.confirmation ({phoneNumber, authNumber, phAuthTransactionId}) completes verification.
  name: end-user-phone-otp
  sources:
  - https://github.com/UshurInc/UshurNodeSDK#usage
  type: otp
slug: ushur-authentication
source_filename: ushur-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/UshurInc/UshurNodeSDK\ndocs: https://docs.ushur.com\nnotes: Ushur publishes no public OpenAPI, so this profile is taken from the\n  official UshurNodeSDK (UshurInc GitHub org) README and examples. The full\n  API documentation at docs.ushur.com sits behind a customer login.\nsummary:\n  types:\n  - session-login\n  - otp\n  notes: Platform clients authenticate by logging in to their tenant host with\n    account email and password; the session established by login is then used\n    for subsequent API calls (initEngagement, getResponses, enterprise data\n    operations). A separate end-user phone-number authentication flow issues\n    an OTP (authentication request returning a phAuthTransactionId, followed\n    by a confirmation call with the received auth number).\nschemes:\n- name: platform-login\n  type: session\n  description: Email + password login against the tenant API host (for example\n    https://apidev.ushur.me/\
  \ in SDK examples; production tenants use their own\n    *.ushur.me host). Emits loginSuccess/loginFailure; all subsequent SDK calls\n    reuse the authenticated session.\n  sources:\n  - https://github.com/UshurInc/UshurNodeSDK#usage\n- name: end-user-phone-otp\n  type: otp\n  description: Two-step end-user verification. ushur.authentication({phoneNumber})\n    triggers an OTP and returns a phAuthTransactionId; ushur.confirmation\n    ({phoneNumber, authNumber, phAuthTransactionId}) completes verification.\n  sources:\n  - https://github.com/UshurInc/UshurNodeSDK#usage\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ushur/refs/heads/main/authentication/ushur-authentication.yml
summary_line: session-login/otp · 2 schemes
tags:
- Company
- Artificial Intelligence
- Customer Experience
- Automation
- Healthcare
- Insurance
- Financial Services
- Agents
---
