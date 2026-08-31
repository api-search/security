---
api_key_in:
- metadata
auth_types:
- bearer
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Toit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Toit secures its APIs with bearer and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Toit
provider_slug: toit
scheme_count: 2
schemes:
- description: Auth.Login exchanges username/password for an access_token (token_type "bearer") plus a refresh_token; Auth.Refresh renews it. Presented on the gRPC authorization metadata for subsequent calls.
  name: bearerToken
  scheme: bearer
  source: grpc/toit-auth.proto
  type: http
- description: Organization-scoped API keys created via OrganizationService.CreateAPIKey / GetAPIKeySecret, used for programmatic (non-interactive) access to the platform.
  in: metadata
  name: apiKey
  source: grpc/toit-organization.proto
  type: apiKey
slug: toit-authentication
source_filename: toit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: grpc/toit-auth.proto + grpc/toit-organization.proto\nnotes: >-\n  Derived from the legacy Toit cloud gRPC API definitions (toitware/api). The open-source\n  Toit SDK and Jaguar (`jag`) developer tooling authenticate to devices locally over WiFi\n  and require no cloud credentials. The cloud platform used two mechanisms below.\nsummary:\n  types: [bearer, apiKey]\n  api_key_in: [metadata]\n  oauth2_flows: []\nschemes:\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    source: grpc/toit-auth.proto\n    description: >-\n      Auth.Login exchanges username/password for an access_token (token_type \"bearer\")\n      plus a refresh_token; Auth.Refresh renews it. Presented on the gRPC authorization\n      metadata for subsequent calls.\n  - name: apiKey\n    type: apiKey\n    in: metadata\n    source: grpc/toit-organization.proto\n    description: >-\n      Organization-scoped API keys created via OrganizationService.CreateAPIKey\
  \ /\n      GetAPIKeySecret, used for programmatic (non-interactive) access to the platform.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toit/refs/heads/main/authentication/toit-authentication.yml
summary_line: bearer/apiKey · 2 schemes
tags:
- Company
- Saas
- IoT
- Embedded
- ESP32
- Microcontrollers
- Programming Language
- Fleet Management
- Firmware
- Developer Tools
- gRPC
---
