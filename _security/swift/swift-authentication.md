---
api_key_in: []
api_specs:
- filename: swift-swiftref-api-openapi.yml
  format: yaml
  label: SwiftRef API
  slug: swiftref-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swift/refs/heads/main/openapi/swift-swiftref-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Swift Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: SWIFT secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: SWIFT
provider_slug: swift
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 2
    tokenUrl: https://api.swift.com/oauth2/v1/token
  name: OAuth2
  sources:
  - openapi/swift-swiftref-api-openapi.yml
  type: oauth2
slug: swift-authentication
source_filename: swift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/swift-swiftref-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://api.swift.com/oauth2/v1/token\n    scopes: 2\n  sources:\n  - openapi/swift-swiftref-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swift/refs/heads/main/authentication/swift-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Banking
- Cross-Border Payments
- Financial Messaging
- Financial Services
- GPI
- ISO 20022
- Payments
---
