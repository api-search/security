---
api_key_in:
- query
api_specs:
- filename: yubico-yubicloud-openapi.yml
  format: yaml
  label: Yubico YubiCloud OTP Validation API
  slug: yubico-yubicloud-otp-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yubico/refs/heads/main/openapi/yubico-yubicloud-openapi.yml
auth_types:
- apiKey
- hmac-signature
description: ''
kind: authentication
layout: security
method: searched
name: Yubico Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yubico secures its APIs with apiKey and hmac-signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Yubico
provider_slug: yubico
scheme_count: 2
schemes:
- description: Numeric Client ID issued free by the Yubico API key generator (https://upgrade.yubico.com/getapikey/).
  in: query
  name: clientId
  parameter: id
  sources:
  - openapi/yubico-yubicloud-openapi.yml
  type: apiKey
- algorithm: HMAC-SHA1
  description: Base64 HMAC-SHA1 signature of the sorted request parameters, computed with the shared secret issued alongside the Client ID. Clients must also verify the signature on the response.
  in: query
  name: requestSignature
  parameter: h
  sources:
  - https://developers.yubico.com/OTP/Specifications/OTP_validation_protocol.html
  type: hmac
slug: yubico-authentication
source_filename: yubico-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developers.yubico.com/OTP/Specifications/OTP_validation_protocol.html\nsummary:\n  types: [apiKey, hmac-signature]\n  api_key_in: [query]\n  oauth2_flows: []\nschemes:\n  - name: clientId\n    type: apiKey\n    in: query\n    parameter: id\n    description: >-\n      Numeric Client ID issued free by the Yubico API key generator\n      (https://upgrade.yubico.com/getapikey/).\n    sources: [openapi/yubico-yubicloud-openapi.yml]\n  - name: requestSignature\n    type: hmac\n    algorithm: HMAC-SHA1\n    in: query\n    parameter: h\n    description: >-\n      Base64 HMAC-SHA1 signature of the sorted request parameters, computed with\n      the shared secret issued alongside the Client ID. Clients must also verify\n      the signature on the response.\n    sources: [https://developers.yubico.com/OTP/Specifications/OTP_validation_protocol.html]\ndocs: https://developers.yubico.com/OTP/Specifications/OTP_validation_protocol.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yubico/refs/heads/main/authentication/yubico-authentication.yml
summary_line: apiKey/hmac-signature · 2 schemes
tags:
- Company
- Enterprise
- Authentication
- Security
- Identity
- Hardware Security
- FIDO2
- WebAuthn
- One-Time Password
---
