---
api_key_in: []
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Hiscox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hiscox secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hiscox
provider_slug: hiscox
scheme_count: 2
schemes:
- authorization_url: unknown
  documented: true
  evidence: 'FAQ, Security section: "What is your API authentication protocol? We authenticate using OAuth 2.0"'
  flows: unknown
  name: oauth2
  scopes_published: false
  source: https://developer.hiscox.com/frequently-asked-questions
  token_url: unknown
  type: oauth2
- documented: true
  evidence: 'API Terms of Use, clause 4 (API Key): "Once registered, Hiscox makes the API Services available to You electronically, requiring an API key for You to access and use the API Services." Issued on partner registration; the holder must keep it confidential and report suspected compromise to Hiscox.'
  in: unknown
  name: api_key
  parameter_name: unknown
  source: https://developer.hiscox.com/terms-use
  type: apiKey
slug: hiscox-authentication
source_filename: hiscox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://developer.hiscox.com/frequently-asked-questions\ndocs:\n- https://developer.hiscox.com/frequently-asked-questions\n- https://developer.hiscox.com/terms-use\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  transport_security: TLS 1.2 only\n  derived_from_openapi: false\n  note: >-\n    No OpenAPI or Swagger document is publicly retrievable, so this profile is\n    searched from the provider's own public FAQ and API Terms of Use rather than\n    derived from a specification. Flow names, token endpoints, scopes and the\n    API-key parameter location are not published and were not inferred.\nschemes:\n- name: oauth2\n  type: oauth2\n  documented: true\n  flows: unknown\n  authorization_url: unknown\n  token_url: unknown\n  scopes_published: false\n  source: https://developer.hiscox.com/frequently-asked-questions\n  evidence: >-\n    FAQ, Security section: \"What is your API authentication protocol? We\n    authenticate using\
  \ OAuth 2.0\"\n- name: api_key\n  type: apiKey\n  documented: true\n  in: unknown\n  parameter_name: unknown\n  source: https://developer.hiscox.com/terms-use\n  evidence: >-\n    API Terms of Use, clause 4 (API Key): \"Once registered, Hiscox makes the API\n    Services available to You electronically, requiring an API key for You to\n    access and use the API Services.\" Issued on partner registration; the holder\n    must keep it confidential and report suspected compromise to Hiscox.\ntransport:\n  tls_minimum: '1.2'\n  tls_maximum: '1.2'\n  environments:\n  - SDBX (sandbox)\n  - Production\n  evidence: >-\n    FAQ, Security section: \"For both SDBX and Production we require TLS 1.2\n    implementation\" and \"We currently ONLY support TLS 1.2.\"\n  observed:\n  - host: api.hiscox.com\n    negotiated_protocol: TLSv1.2\n    probed: '2026-07-25'\n    note: Live TLS handshake against the gateway host corroborates the TLS 1.2 policy.\ncredential_issuance:\n  self_serve: false\n  process:\
  \ >-\n    Credentials are not self-serve. A Hiscox Partnership Manager must approve the\n    commercial partnership first; on approval an account is created that grants\n    immediate access to the SDBX sandbox. Lost credentials are recovered through\n    the Login page password reset, or by contacting the Partnership Manager.\n  contacts:\n  - hiscox.partneroperations@hiscox.com\n  - partnercontact@hiscox.com\n  evidence:\n  - >-\n    FAQ, Registration section: \"Once approved by our Partnership Manager an\n    account will be created for you, which gives you immediate access to SDBX\"\n    and \"Access is provided to our authorized partners only.\"\n  - >-\n    API Terms of Use, clause 3 (Enrollment): \"In order to access and use the API\n    Services, You must be approved by Hiscox and registered in Hiscox's API\n    Portal.\"\ngaps:\n- Token endpoint and OAuth 2.0 grant type are not published.\n- No scope or permission reference is published, so scopes/ is intentionally absent.\n-\
  \ API-key transport (header vs query) is not published.\n- No /.well-known/oauth-authorization-server or /.well-known/openid-configuration is served (all 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hiscox/refs/heads/main/authentication/hiscox-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Insurance
- United Kingdom
- Property and Casualty
- Specialty Insurance
- Cyber Insurance
- Underwriting
- Reinsurance
- Lloyd's of London
- Small Business Insurance
- Quotes
- ACORD
- Carrier
- Cargo
- Marine
- Payments
- API Gateway
---
