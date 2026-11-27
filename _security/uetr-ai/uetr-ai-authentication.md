---
anonymous_access: false
api_key_in: []
api_specs:
- filename: uetr-ai-account-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Account API
  slug: uetr-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-account-api-openapi.yml
- filename: uetr-ai-owner-confirmation-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Owner confirmation API
  slug: uetr-ai-owner-confirmation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-owner-confirmation-api-openapi.yml
- filename: uetr-ai-payment-records-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Payment records API
  slug: uetr-ai-payment-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-payment-records-api-openapi.yml
- filename: uetr-ai-team-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Team API
  slug: uetr-ai-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-team-api-openapi.yml
- filename: uetr-ai-transfers-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Transfers API
  slug: uetr-ai-transfers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-transfers-api-openapi.yml
- filename: uetr-ai-webhooks-api-openapi.yml
  format: yaml
  label: SWIFT UETR Tracker Webhooks API
  slug: uetr-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uetr-ai/openapi/uetr-ai-webhooks-api-openapi.yml
auth_types: []
description: Authentication methods for the uetr.ai API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: uetr.ai - UETR and SWIFT Payment Tracking Authentication
name_suffix: Authentication
oauth_flows: []
overview: uetr.ai - UETR and SWIFT Payment Tracking declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: uetr.ai - UETR and SWIFT Payment Tracking
provider_slug: uetr-ai
scheme_count: 2
schemes:
- evidence: 'Send the key only in the Authorization header: curl "https://uetr.ai/api/v1/account" \ -H "Authorization: Bearer $UETR_API_KEY"'
  header: Authorization
  how_to_obtain: Create keys on the MCP and API page of uetr.ai.
  location: header
  name: Bearer
  type: http-bearer
- evidence: Claude, ChatGPT and other AI apps connect to https://uetr.ai/mcp and sign in through https://auth.uetr.ai with OAuth 2.1 and PKCE
  how_to_obtain: Sign in through https://auth.uetr.ai; the person approves the app on uetr.ai and the app receives its own tokens.
  name: OAuth 2.1 PKCE
  type: oauth2
slug: uetr-ai-authentication
source_filename: uetr-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://uetr.ai/docs/api/authentication
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://uetr.ai/docs/api/authentication\nsources:\n- https://uetr.ai/docs/api/authentication\n- https://uetr.ai/docs/api/authentication.md\n- https://uetr.ai/docs/api/rotate-webhook-secret\n- https://uetr.ai/mcp.md\ndescription: Authentication methods for the uetr.ai API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send the key only in the Authorization header: curl \"https://uetr.ai/api/v1/account\" \\ -H \"Authorization: Bearer $UETR_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys on the MCP and API page of uetr.ai.\n- type: oauth2\n  name: OAuth 2.1 PKCE\n  evidence: Claude, ChatGPT and other AI apps connect to https://uetr.ai/mcp and sign in through https://auth.uetr.ai with OAuth 2.1 and PKCE\n  how_to_obtain: Sign in through https://auth.uetr.ai; the person approves the app on uetr.ai and the app receives its own tokens.\n\
  docs: https://uetr.ai/docs/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/uetr-ai/authentication/uetr-ai-authentication.yml
summary_line: 2 schemes
tags:
- Payments
- SWIFT
- Tracking
- Financial Services
---
