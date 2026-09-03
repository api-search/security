---
api_key_in:
- header
api_specs:
- filename: ametek-powervar-isite-pro-openapi.yml
  format: yaml
  label: AMETEK Powervar iSite PRO REST API
  slug: powervar-isite-pro
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ametek/refs/heads/main/openapi/ametek-powervar-isite-pro-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ametek Authentication
name_suffix: Authentication
oauth_flows: []
overview: AMETEK secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AMETEK
provider_slug: ametek
scheme_count: 2
schemes:
- description: HTTP Basic Authentication, as published. Authentication is required for access to all API features. Credentials are the adapter's own local administrative credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/ametek-powervar-isite-pro-openapi.yml
  type: http
- description: Web session token issued by the adapter's own web interface and presented in the `x-auth-token` header, as published.
  in: header
  name: sessionToken
  parameter: x-auth-token
  sources:
  - openapi/ametek-powervar-isite-pro-openapi.yml
  type: apiKey
slug: ametek-authentication
source_filename: ametek-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://www.powervar.com/-/media/ametekpowervar/pdf/products/connectivity-solutions/isite-pro/user-manuals/a55-00202-rev-b-isite-pro-rest-api-definition.pdf\ndocs: https://www.powervar.com/-/media/ametekpowervar/pdf/products/connectivity-solutions/isite-pro/user-manuals/a55-00202-rev-b-isite-pro-rest-api-definition.pdf\nnote: >-\n  Read from AMETEK Powervar's own published REST API definition (A55-00202 REV B), which states\n  verbatim: \"Basic Authentication supported\", \"Web session tokens supported using x-auth-token\n  header\", and \"Authentication is required for access to all API features\". The OpenAPI in\n  openapi/ was transcribed from that same document, so the spec and the docs are one source.\n  No OAuth2, OIDC or mTLS is published for this surface. Credentials are the adapter's own local\n  administrative credentials, issued by the device, not by an AMETEK-operated identity service.\nsummary:\n  types:\n  - apiKey\n\
  \  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication, as published. Authentication is required for access\n    to all API features. Credentials are the adapter's own local administrative credentials.\n  sources:\n  - openapi/ametek-powervar-isite-pro-openapi.yml\n- name: sessionToken\n  type: apiKey\n  in: header\n  parameter: x-auth-token\n  description: Web session token issued by the adapter's own web interface and presented in\n    the `x-auth-token` header, as published.\n  sources:\n  - openapi/ametek-powervar-isite-pro-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ametek/refs/heads/main/authentication/ametek-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Electronic Instruments
- Test and Measurement
- Aerospace
- Energy
- Industrial
- Medical Instruments
- Precision Motion Control
- Manufacturing
- Fortune 1000
---
