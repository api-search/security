---
api_key_in: []
api_specs:
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Verification Requests API
  slug: evident-id-verification-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Attributes & Credentials API
  slug: evident-id-attributes-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Identity Assurance API
  slug: evident-id-identity-assurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Insurance & COI Verification API
  slug: evident-id-insurance-coi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Results API
  slug: evident-id-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
- filename: evident-id-openapi.yml
  format: yaml
  label: Evident Webhooks API
  slug: evident-id-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/openapi/evident-id-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Evident Id Authentication
name_suffix: Authentication
oauth_flows: []
overview: Evident secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Evident
provider_slug: evident-id
scheme_count: 2
schemes:
- description: HTTP Basic Auth using your Evident username and API key (VerifyAPI).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/evident-id-openapi.yml
  type: http
- description: Bearer token using the userIdentityToken returned by VerifyAPI (SubmitAPI).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/evident-id-openapi.yml
  type: http
slug: evident-id-authentication
source_filename: evident-id-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/evident-id-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using your Evident username and API key (VerifyAPI).\n  sources:\n  - openapi/evident-id-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token using the userIdentityToken returned by VerifyAPI (SubmitAPI).\n  sources:\n  - openapi/evident-id-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evident-id/refs/heads/main/authentication/evident-id-authentication.yml
summary_line: http · 2 schemes
tags:
- Identity Verification
- Credential Verification
- Background Check
- Insurance Verification
- COI
---
