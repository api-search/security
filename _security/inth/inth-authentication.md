---
api_key_in: []
api_specs:
- filename: inth-c15t-consent-api.yml
  format: yaml
  label: c15t Consent Backend API
  slug: c15t-consent-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inth/refs/heads/main/openapi/inth-c15t-consent-api.yml
auth_types: []
description: The c15t consent backend authenticates server-side requests with a Bearer API key. Browser-facing endpoints (init, status) are public and unauthenticated so the client SDK can bootstrap a banner without exposing a secret.
kind: authentication
layout: security
method: searched
name: Inth Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inth declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Inth
provider_slug: inth
scheme_count: 1
schemes:
- applies_to:
  - GET /subjects (list by external ID)
  - PUT /legal-documents/{type}/current
  description: Secret API key passed as a Bearer token. Keys are provisioned per instance (inth.com dashboard) or configured for self-hosted deployments. The extractBearerToken middleware requires the literal "Bearer " prefix.
  format: Bearer [example key]<key>
  header: Authorization
  id: bearerAuth
  location: header
  scheme: bearer
  type: http
slug: inth-authentication
source_filename: inth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  github.com/c15t/c15t packages/backend/src/middleware/auth/validate-api-key.ts\n  and c15t.com/docs/self-host. Auth profile derived from the open-source backend\n  and confirmed against docs.\ndescription: >-\n  The c15t consent backend authenticates server-side requests with a Bearer API\n  key. Browser-facing endpoints (init, status) are public and unauthenticated so\n  the client SDK can bootstrap a banner without exposing a secret.\ndocs: https://c15t.com/docs/self-host\nschemes:\n  - id: bearerAuth\n    type: http\n    scheme: bearer\n    location: header\n    header: Authorization\n    format: \"Bearer [example key]<key>\"\n    description: >-\n      Secret API key passed as a Bearer token. Keys are provisioned per instance\n      (inth.com dashboard) or configured for self-hosted deployments. The\n      extractBearerToken middleware requires the literal \"Bearer \" prefix.\n    applies_to:\n      - GET /subjects\
  \ (list by external ID)\n      - PUT /legal-documents/{type}/current\npublic_endpoints:\n  - GET /init\n  - GET /status\n  - GET /spec.json\noauth2: false\nopenid_connect: false\nmutual_tls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inth/refs/heads/main/authentication/inth-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Consent Management
- Privacy
- Cookie Consent
- GDPR
- CCPA
- Compliance
- Consent
- Developer Tools
- Open Source
---
