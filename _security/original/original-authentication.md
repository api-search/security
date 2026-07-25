---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Original Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bodygram declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Bodygram
provider_slug: original
scheme_count: 4
schemes:
- description: Secret API key issued from the Account page at platform.bodygram.com, sent as a bearer token in the Authorization header for all server-side Platform API calls.
  first_party: true
  id: api-key
  in: header
  name: Authorization
  scheme: bearer
  type: http
- description: Organization identifier that scopes every /api/orgs/{ORG_ID}/... resource path.
  id: organization-id
  in: path
  name: ORG_ID
  type: apiKey
- description: Short-lived scan token (issued by POST /api/orgs/{ORG_ID}/scan-tokens) that authorizes the hosted Bodygram Scanner from the browser without exposing the secret API key.
  id: scan-token
  in: header
  name: Authorization
  type: apiKey
- description: Domain-restricted public key that authenticates the browser-side Body2Fit widget.
  first_party: true
  id: client-key
  in: config
  name: clientKey
  type: apiKey
slug: original-authentication
source_filename: original-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.bodygram.com/platform/api-reference\ndocs: https://docs.bodygram.com/platform/api-reference\napi: Bodygram Platform API\nsummary: >-\n  Server-to-server requests authenticate with a secret API key passed as a bearer\n  token in the Authorization header; every Platform resource path is scoped to an\n  Organization ID. Browser-side Body2Fit widgets authenticate with a domain-restricted\n  public clientKey instead of the secret key.\nschemes:\n- id: api-key\n  type: http\n  scheme: bearer\n  in: header\n  name: Authorization\n  first_party: true\n  description: >-\n    Secret API key issued from the Account page at platform.bodygram.com, sent as a\n    bearer token in the Authorization header for all server-side Platform API calls.\n- id: organization-id\n  type: apiKey\n  in: path\n  name: ORG_ID\n  description: >-\n    Organization identifier that scopes every /api/orgs/{ORG_ID}/... resource path.\n- id: scan-token\n\
  \  type: apiKey\n  in: header\n  name: Authorization\n  description: >-\n    Short-lived scan token (issued by POST /api/orgs/{ORG_ID}/scan-tokens) that\n    authorizes the hosted Bodygram Scanner from the browser without exposing the\n    secret API key.\n- id: client-key\n  type: apiKey\n  in: config\n  name: clientKey\n  first_party: true\n  description: >-\n    Domain-restricted public key that authenticates the browser-side Body2Fit widget.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/original/refs/heads/main/authentication/original-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Body Measurement
- Computer Vision
- Artificial Intelligence
- Sizing
- Retail
- 3D Avatar
- Health
- SDK
---
