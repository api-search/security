---
api_key_in: []
api_specs:
- filename: descope-apps-api-openapi.yml
  format: yaml
  label: Descope Apps API
  slug: descope-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-apps-api-openapi.yml
- filename: descope-auth-api-openapi.yml
  format: yaml
  label: Descope Auth API
  slug: descope-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-auth-api-openapi.yml
- filename: descope-custom-attributes-api-openapi.yml
  format: yaml
  label: Descope Custom Attributes API
  slug: descope-custom-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-custom-attributes-api-openapi.yml
- filename: descope-default-api-openapi.yml
  format: yaml
  label: Descope Default API
  slug: descope-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-default-api-openapi.yml
- filename: descope-email-api-openapi.yml
  format: yaml
  label: Descope Email API
  slug: descope-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-email-api-openapi.yml
- filename: descope-embedded-link-api-openapi.yml
  format: yaml
  label: Descope Embedded Link API
  slug: descope-embedded-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-embedded-link-api-openapi.yml
- filename: descope-fedcm-api-openapi.yml
  format: yaml
  label: Descope Fedcm API
  slug: descope-fedcm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-fedcm-api-openapi.yml
- filename: descope-instant-message-im-api-openapi.yml
  format: yaml
  label: Descope Instant Message (IM) API
  slug: descope-instant-message-im-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-instant-message-im-api-openapi.yml
- filename: descope-keys-api-openapi.yml
  format: yaml
  label: Descope Keys API
  slug: descope-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-keys-api-openapi.yml
- filename: descope-mgmt-api-openapi.yml
  format: yaml
  label: Descope Mgmt API
  slug: descope-mgmt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-mgmt-api-openapi.yml
- filename: descope-oauth2-api-openapi.yml
  format: yaml
  label: Descope Oauth2 API
  slug: descope-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-oauth2-api-openapi.yml
- filename: descope-scim-api-openapi.yml
  format: yaml
  label: Descope Scim API
  slug: descope-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-scim-api-openapi.yml
- filename: descope-text-message-sms-api-openapi.yml
  format: yaml
  label: Descope Text Message (SMS) API
  slug: descope-text-message-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-text-message-sms-api-openapi.yml
- filename: descope-verification-api-openapi.yml
  format: yaml
  label: Descope Verification API
  slug: descope-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-verification-api-openapi.yml
- filename: descope-voice-message-phone-api-openapi.yml
  format: yaml
  label: Descope Voice Message (Phone) API
  slug: descope-voice-message-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-voice-message-phone-api-openapi.yml
- filename: descope-well-known-api-openapi.yml
  format: yaml
  label: Descope .well Known API
  slug: descope-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/openapi/descope-well-known-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Descope Authentication
name_suffix: Authentication
oauth_flows: []
overview: Descope secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Descope
provider_slug: descope
scheme_count: 1
schemes:
- bearerFormat: Project ID
  description: Project ID as bearer token.
  name: Descope Project ID
  scheme: bearer
  sources:
  - openapi/descope-openapi.yml
  type: http
slug: descope-authentication
source_filename: descope-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/descope-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Descope Project ID\n  type: http\n  scheme: bearer\n  bearerFormat: Project ID\n  description: Project ID as bearer token.\n  sources:\n  - openapi/descope-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/descope/refs/heads/main/authentication/descope-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Identity
- CIAM
- Passwordless
- Passkeys
- MFA
- SSO
- OIDC
- SAML
- SCIM
- Authorization
- FGA
- Agentic Identity
- MCP
---
