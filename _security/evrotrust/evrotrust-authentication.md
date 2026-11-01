---
anonymous_access: false
api_key_in: []
api_specs:
- filename: evrotrust-all-signing-api-openapi.yml
  format: yaml
  label: Evrotrust All Signing API
  slug: evrotrust-all-signing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-all-signing-api-openapi.yml
- filename: evrotrust-e-authentication-api-openapi.yml
  format: yaml
  label: Evrotrust E Authentication API
  slug: evrotrust-e-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-e-authentication-api-openapi.yml
- filename: evrotrust-e-delivery-api-openapi.yml
  format: yaml
  label: Evrotrust E Delivery API
  slug: evrotrust-e-delivery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-e-delivery-api-openapi.yml
- filename: evrotrust-e-signatures-api-openapi.yml
  format: yaml
  label: Evrotrust E Signatures API
  slug: evrotrust-e-signatures-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-e-signatures-api-openapi.yml
- filename: evrotrust-evrotrust-eid-registered-users-api-openapi.yml
  format: yaml
  label: Evrotrust Evrotrust eID (Registered Users) API
  slug: evrotrust-evrotrust-eid-registered-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-evrotrust-eid-registered-users-api-openapi.yml
- filename: evrotrust-ident-lite-advanced-basic-api-openapi.yml
  format: yaml
  label: Evrotrust Ident Lite (Advanced, Basic) API
  slug: evrotrust-ident-lite-advanced-basic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-ident-lite-advanced-basic-api-openapi.yml
- filename: evrotrust-one-time-signatures-documents-api-openapi.yml
  format: yaml
  label: Evrotrust One-time Signatures (Documents) API
  slug: evrotrust-one-time-signatures-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-one-time-signatures-documents-api-openapi.yml
- filename: evrotrust-one-time-signatures-hash-api-openapi.yml
  format: yaml
  label: Evrotrust One-time Signatures (Hash) API
  slug: evrotrust-one-time-signatures-hash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-one-time-signatures-hash-api-openapi.yml
- filename: evrotrust-signing-via-app-sdk-documents-api-openapi.yml
  format: yaml
  label: Evrotrust Signing via App/SDK (Documents) API
  slug: evrotrust-signing-via-app-sdk-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-signing-via-app-sdk-documents-api-openapi.yml
- filename: evrotrust-signing-via-app-sdk-hash-api-openapi.yml
  format: yaml
  label: Evrotrust Signing via App/SDK (Hash) API
  slug: evrotrust-signing-via-app-sdk-hash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evrotrust/openapi/evrotrust-signing-via-app-sdk-hash-api-openapi.yml
auth_types: []
description: API authentication uses HMAC-SHA256 signature scheme where the request body is signed with a secret derived from an API key, and the signature is sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Evrotrust Authentication
name_suffix: Authentication
oauth_flows: []
overview: Evrotrust declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Evrotrust
provider_slug: evrotrust
scheme_count: 1
schemes:
- evidence: On every request you have to set a header parameter "Authorization". Thus we proof that the request came from you and wasn’t changed in transit. So you sign the exact request body with a secret derived from your API key, and send that in the Authorization header.
  header: Authorization
  how_to_obtain: 'You need below credentials from Evrotrust (technical_support@evrotrust.com): - API key (secret) - Vendor Number (your unique company ID, which goes inside the JSON body)'
  location: header
  name: HMAC-SHA256 Authorization
  type: hmac
slug: evrotrust-authentication
source_filename: evrotrust-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.evrotrust.com/docs/e-authentication.md
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (deepseek)\nsource: https://docs.evrotrust.com/docs/e-authentication.md\nsources:\n- https://docs.evrotrust.com/docs/e-authentication.md\n- https://docs.evrotrust.com/reference/authentication-1.md\n- https://docs.evrotrust.com/reference/authentication-1\ndescription: API authentication uses HMAC-SHA256 signature scheme where the request body is signed with a secret derived from an API key, and\n  the signature is sent in the Authorization header.\nschemes:\n- type: hmac\n  name: HMAC-SHA256 Authorization\n  evidence: On every request you have to set a header parameter \"Authorization\". Thus we proof that the request came from you and wasn’t changed\n    in transit. So you sign the exact request body with a secret derived from your API key, and send that in the Authorization header.\n  header: Authorization\n  location: header\n  how_to_obtain: 'You need below credentials from Evrotrust (technical_support@evrotrust.com):\
  \ - API key (secret) - Vendor Number (your unique\n    company ID, which goes inside the JSON body)'\ndocs: https://docs.evrotrust.com/docs/e-authentication.md, https://docs.evrotrust.com/reference/authentication-1.md\nnote: The e-Authentication page describes user authentication flow (MFA via Evrotrust app), not API client authentication. The API authentication\n  is documented in the Authorization header page.\n"
source_yaml_url: https://artifacts.apis.io/evrotrust/authentication/evrotrust-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Trust Services
- Electronic Signatures
- Digital Identity
- eIDAS
- KYC
- Identity Verification
- Timestamping
- Compliance
---
