---
api_key_in:
- header
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cloudkit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apple CloudKit secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Apple CloudKit
provider_slug: cloudkit
scheme_count: 2
schemes:
- description: 'CloudKit API token issued from the CloudKit dashboard, appended to

    the request URL as `ckAPIToken`. Required for end-user authenticated

    access via web auth tokens.'
  in: query
  name: cloudKitApiToken
  parameter: ckAPIToken
  sources:
  - openapi/cloudkit-openapi.yml
  type: apiKey
- description: 'Server-to-server authentication uses ECDSA-signed requests with

    `X-Apple-CloudKit-Request-KeyID`, `X-Apple-CloudKit-Request-ISO8601Date`,

    and `X-Apple-CloudKit-Request-SignatureV1` headers.'
  in: header
  name: serverToServer
  parameter: X-Apple-CloudKit-Request-SignatureV1
  sources:
  - openapi/cloudkit-openapi.yml
  type: apiKey
slug: cloudkit-authentication
source_filename: cloudkit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloudkit-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: cloudKitApiToken\n  type: apiKey\n  in: query\n  parameter: ckAPIToken\n  description: |-\n    CloudKit API token issued from the CloudKit dashboard, appended to\n    the request URL as `ckAPIToken`. Required for end-user authenticated\n    access via web auth tokens.\n  sources:\n  - openapi/cloudkit-openapi.yml\n- name: serverToServer\n  type: apiKey\n  in: header\n  parameter: X-Apple-CloudKit-Request-SignatureV1\n  description: |-\n    Server-to-server authentication uses ECDSA-signed requests with\n    `X-Apple-CloudKit-Request-KeyID`, `X-Apple-CloudKit-Request-ISO8601Date`,\n    and `X-Apple-CloudKit-Request-SignatureV1` headers.\n  sources:\n  - openapi/cloudkit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudkit/refs/heads/main/authentication/cloudkit-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Apple
- Cloud Storage
- CloudKit
- Database
- iCloud
- Mobile
- Sync
- Web Services
---
