---
api_key_in:
- header
api_specs:
- filename: cover-genius-openapi.yml
  format: yaml
  label: XCover Offers API
  slug: xcover-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cover-genius/refs/heads/main/openapi/cover-genius-openapi.yml
- filename: cover-genius-openapi.yml
  format: yaml
  label: XCover Bookings and Policies API
  slug: xcover-bookings-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cover-genius/refs/heads/main/openapi/cover-genius-openapi.yml
- filename: cover-genius-openapi.yml
  format: yaml
  label: XClaim Claims API
  slug: xclaim-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cover-genius/refs/heads/main/openapi/cover-genius-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cover Genius Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cover Genius secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cover Genius
provider_slug: cover-genius
scheme_count: 1
schemes:
- description: HTTP Signature authentication. Each request carries an X-Api-Key header, a Date header (RFC 822 GMT), and an Authorization header of the form Signature keyId="{API_KEY}",algorithm="hmac-sha512",signature="{base64}". The signature is an HMAC of the canonical string (by default the date header) computed with the partner's secret key.
  in: header
  name: XCoverSignature
  parameter: Authorization
  sources:
  - openapi/cover-genius-openapi.yml
  type: apiKey
slug: cover-genius-authentication
source_filename: cover-genius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cover-genius-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: XCoverSignature\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: HTTP Signature authentication. Each request carries an X-Api-Key header, a Date\n    header (RFC 822 GMT), and an Authorization header of the form Signature keyId=\"{API_KEY}\",algorithm=\"hmac-sha512\",signature=\"{base64}\".\n    The signature is an HMAC of the canonical string (by default the date header) computed with\n    the partner's secret key.\n  sources:\n  - openapi/cover-genius-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cover-genius/refs/heads/main/authentication/cover-genius-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Insurance
- Insurtech
- Embedded Insurance
- Protection
- Claims
---
