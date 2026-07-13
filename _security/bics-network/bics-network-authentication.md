---
api_key_in: []
api_specs:
- filename: bics-sms-openapi.json
  format: json
  label: BICS SMS API
  slug: bics-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-sms-openapi.json
- filename: bics-mynumbers-openapi.json
  format: json
  label: BICS MyNumbers API
  slug: bics-mynumbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-mynumbers-openapi.json
- filename: bics-mynumbers-porting-openapi.json
  format: json
  label: BICS MyNumbers Number Porting API
  slug: bics-mynumbers-number-porting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-mynumbers-porting-openapi.json
- filename: bics-mynumbers-cdr-openapi.json
  format: json
  label: BICS MyNumbers CDR API
  slug: bics-mynumbers-cdr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-mynumbers-cdr-openapi.json
- filename: bics-mynumbers-address-management-openapi.json
  format: json
  label: BICS MyNumbers Address Management API
  slug: bics-mynumbers-address-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-mynumbers-address-management-openapi.json
- filename: bics-mynumbers-disconnection-openapi.json
  format: json
  label: BICS MyNumbers Disconnection API
  slug: bics-mynumbers-disconnection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-mynumbers-disconnection-openapi.json
- filename: bics-mynumbers-emergency-services-openapi.json
  format: json
  label: BICS MyNumbers Emergency Services API
  slug: bics-mynumbers-emergency-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-mynumbers-emergency-services-openapi.json
- filename: bics-connect-openapi.json
  format: json
  label: BICS Connect API
  slug: bics-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/openapi/bics-connect-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: ''
name: Bics Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: BICS declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: BICS
provider_slug: bics-network
scheme_count: 0
schemes: []
slug: bics-network-authentication
source_filename: bics-network-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "aid: bics-network\nname: BICS\nauthentication:\n  type: OAuth2\n  scheme: Bearer\n  summary: >-\n    BICS developer-portal APIs are protected with OAuth2. Access is not fully\n    self-serve - a developer registers to consume an API on the portal, the\n    consumption request is approved by BICS (confirmed by email), and the email\n    contains instructions for creating an OAuth2 token. Each request then carries\n    the access token in an Authorization header.\n  tokenModel: OAuth2 access token presented as a Bearer credential in the Authorization request header\n  onboarding: >-\n    Register on developer.bics.com to consume an API, wait for approval, then\n    follow the emailed instructions to generate an OAuth2 token. Sandbox base\n    URLs (sandbox.api.bics.com) are available for the MyNumbers family for\n    testing before production.\n  gatedProducts: >-\n    Mobile identity, number verification, HLR/reachability lookup, SIM-swap and\n    device-location products are\
  \ not exposed on the self-serve portal; they are\n    provisioned through a BICS / Proximus Global commercial agreement with\n    credentials issued per contract.\n  sources:\n  - url: https://developer.bics.com/portal/apis\n    type: Documentation\n    note: Portal API policy states OAuth2 token auth, register-to-consume, approval by email.\n  - url: https://developer.bics.com/portal/welcome\n    type: Documentation\n    note: Access token required in request headers for each API request.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bics-network/refs/heads/main/authentication/bics-network-authentication.yml
summary_line: 0 schemes
tags:
- Number Verification
- Telecom
- Mobile Identity
- Anti-Fraud
- Device Location
- OTP
- SMS
- Numbering
- Number Portability
- Fraud Prevention
- Carrier
- CPaaS
---
