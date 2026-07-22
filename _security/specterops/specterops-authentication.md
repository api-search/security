---
api_key_in:
- header
api_specs:
- filename: specterops-bloodhound-openapi.json
  format: json
  label: BloodHound API
  slug: bloodhound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/specterops/refs/heads/main/openapi/specterops-bloodhound-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Specterops Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpecterOps secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SpecterOps
provider_slug: specterops
scheme_count: 4
schemes:
- bearerFormat: JWT
  description: '`Authorization: Bearer $JWT_TOKEN`'
  name: JWTBearerToken
  scheme: bearer
  sources:
  - openapi/specterops-bloodhound-openapi.json
  type: http
- description: '`Authorization: bhesignature $TOKEN_ID`'
  in: header
  name: SignedRequest
  parameter: Authorization
  sources:
  - openapi/specterops-bloodhound-openapi.json
  type: apiKey
- description: '`RequestDate: $RFC3339_DATETIME`'
  in: header
  name: RequestDate
  parameter: RequestDate
  sources:
  - openapi/specterops-bloodhound-openapi.json
  type: apiKey
- description: '`Signature: $BASE64ENCODED_HMAC_SIGNATURE`'
  in: header
  name: HMACSignature
  parameter: Signature
  sources:
  - openapi/specterops-bloodhound-openapi.json
  type: apiKey
slug: specterops-authentication
source_filename: specterops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/specterops-bloodhound-openapi.json\ndocs: https://bloodhound.specterops.io/integrations/bloodhound-api/working-with-api\nnotes: 'Two mechanisms: JWT bearer (Authorization: Bearer $JWT, 8-hour TTL, via Login) and an HMAC-signed\n  request using a non-expiring API key/ID pair (Authorization: bhesignature $TOKEN_ID + RequestDate +\n  Signature; HMAC-SHA-256 chain over method+URI, RFC3339 date-to-hour, and body).'\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: JWTBearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: '`Authorization: Bearer $JWT_TOKEN`'\n  sources:\n  - openapi/specterops-bloodhound-openapi.json\n- name: SignedRequest\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: '`Authorization: bhesignature $TOKEN_ID`'\n  sources:\n  - openapi/specterops-bloodhound-openapi.json\n- name: RequestDate\n  type: apiKey\n  in: header\n\
  \  parameter: RequestDate\n  description: '`RequestDate: $RFC3339_DATETIME`'\n  sources:\n  - openapi/specterops-bloodhound-openapi.json\n- name: HMACSignature\n  type: apiKey\n  in: header\n  parameter: Signature\n  description: '`Signature: $BASE64ENCODED_HMAC_SIGNATURE`'\n  sources:\n  - openapi/specterops-bloodhound-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/specterops/refs/heads/main/authentication/specterops-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Cybersecurity
- Identity
- Active Directory
- Attack Path Management
- Offensive Security
- Graph
- BloodHound
---
