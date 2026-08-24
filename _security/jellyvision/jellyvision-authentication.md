---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Jellyvision Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jellyvision declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Jellyvision
provider_slug: jellyvision
scheme_count: 2
schemes:
- audience: https://integrated-partner.myalex.com
  bearer_format: JWT
  credentials_issued_per_environment: 2
  credentials_note: Two API keys are issued, one per environment.
  flow: clientCredentials
  id: oauth2_client_credentials
  in: header
  scheme: bearer
  scopes:
  - rw:self
  token_endpoints:
  - environment: production
    url: https://login.myalex.com/oauth/token
  - environment: pre-production
    url: https://login.jellydevs.com/oauth/token
  token_lifetime_note: Documented expires_in is 86400 (24 hours). The docs require partners to cache the token and refresh it every 24 hours or on a 401, and warn that requesting a token per API call will trigger rate limiting.
  token_lifetime_seconds: 86400
  token_request_parameters:
  - name: client_id
    note: Provided by Jellyvision.
    required: true
  - name: client_secret
    note: Provided by Jellyvision.
    required: true
  - name: audience
    note: Provided by Jellyvision; documented value is https://integrated-partner.myalex.com.
    required: true
  - name: grant_type
    note: Always client_credentials.
    required: true
  type: oauth2
- attributes:
  - description: An ID unique to each partner.
    name: partner_id
    supplied_by: Jellyvision
  - description: An ID unique to each customer; may equal partner_id.
    name: partner_client_id
    supplied_by: Jellyvision
  - description: An ID unique to each end user associated with a given partner_id.
    name: partner_user_id
    supplied_by: partner
  - description: An ID representing the plan year the user is accessing.
    name: product_key
    supplied_by: Jellyvision
  - description: A unique visit to the ALEX experience, per user.
    name: session_id
    supplied_by: partner
  - description: The ALEX environment (https://www.myalex.com or https://qa.myalex.com).
    name: target
    supplied_by: partner
  id: saml2_sso
  note: SP-initiated authentication can be supported on request and at Jellyvision's discretion.
  profile: IdP-initiated SSO
  signing:
    certificate: x509 RSA-SHA256
    formats:
    - PEM
    - CER
    key_size_bits: 4096
  type: saml2
slug: jellyvision-authentication
source_filename: jellyvision-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://partner-api-docs.myalex.com/\ndocs: https://partner-api-docs.myalex.com/\nsummary: >-\n  The ALEX Partner Integration API uses OAuth 2.0 client credentials against a Jellyvision Auth0\n  tenant to mint a short-lived bearer JWT, then requires four partner-identity headers plus a product\n  key on every call. A separate SAML 2.0 IdP-initiated single sign-on flow carries the end user into\n  the ALEX experience itself. There is no API-key, basic-auth or mTLS option documented.\nschemes:\n- id: oauth2_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  in: header\n  scheme: bearer\n  bearer_format: JWT\n  token_endpoints:\n  - environment: production\n    url: https://login.myalex.com/oauth/token\n  - environment: pre-production\n    url: https://login.jellydevs.com/oauth/token\n  audience: https://integrated-partner.myalex.com\n  token_request_parameters:\n  - name: client_id\n    required: true\n    note:\
  \ Provided by Jellyvision.\n  - name: client_secret\n    required: true\n    note: Provided by Jellyvision.\n  - name: audience\n    required: true\n    note: Provided by Jellyvision; documented value is https://integrated-partner.myalex.com.\n  - name: grant_type\n    required: true\n    note: Always client_credentials.\n  token_lifetime_seconds: 86400\n  token_lifetime_note: >-\n    Documented expires_in is 86400 (24 hours). The docs require partners to cache the token and\n    refresh it every 24 hours or on a 401, and warn that requesting a token per API call will\n    trigger rate limiting.\n  scopes:\n  - rw:self\n  credentials_issued_per_environment: 2\n  credentials_note: Two API keys are issued, one per environment.\n- id: saml2_sso\n  type: saml2\n  profile: IdP-initiated SSO\n  note: >-\n    SP-initiated authentication can be supported on request and at Jellyvision's discretion.\n  signing:\n    certificate: x509 RSA-SHA256\n    key_size_bits: 4096\n    formats:\n    - PEM\n\
  \    - CER\n  attributes:\n  - name: partner_id\n    supplied_by: Jellyvision\n    description: An ID unique to each partner.\n  - name: partner_client_id\n    supplied_by: Jellyvision\n    description: An ID unique to each customer; may equal partner_id.\n  - name: partner_user_id\n    supplied_by: partner\n    description: An ID unique to each end user associated with a given partner_id.\n  - name: product_key\n    supplied_by: Jellyvision\n    description: An ID representing the plan year the user is accessing.\n  - name: session_id\n    supplied_by: partner\n    description: A unique visit to the ALEX experience, per user.\n  - name: target\n    supplied_by: partner\n    description: The ALEX environment (https://www.myalex.com or https://qa.myalex.com).\nrequired_request_headers:\n- name: Authorization\n  value_form: 'Bearer <jwt>'\n  required: true\n- name: Partner-Id\n  required: true\n  description: An ID unique to each partner.\n- name: Partner-Client-Id\n  required: true\n  description:\
  \ An ID unique to each customer.\n- name: Partner-User-Id\n  required: true\n  description: An ID unique to each end user.\n- name: Product-Key\n  required: true\n  description: Plan-year key supplied by Jellyvision.\n- name: Accept-Version\n  required: false\n  default: v1\n  description: API version selector; v1 when omitted.\nidentity_providers:\n  production:\n    issuer: https://login.myalex.com/\n    platform: Auth0\n    discovery: /.well-known/openid-configuration (HTTP 200, saved)\n  pre_production:\n    issuer: https://login.jellydevs.com/\n    platform: Auth0\n    discovery: /.well-known/openid-configuration (HTTP 200, saved)\ncredential_issuance: >-\n  Client ID, client secret, audience, Partner-Id, Partner-Client-Id and Product-Key are all issued by\n  Jellyvision as part of partner onboarding. There is no self-service signup for the Partner\n  Integration API; the public entry point is https://www.jellyvision.com/get-a-demo/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jellyvision/refs/heads/main/authentication/jellyvision-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Employee Benefits
- Human Resources
- Benefits Administration
- Benefits Enrollment
- Health Insurance
- Decision Support
- HR Technology
- Insurance
- Employee Engagement
---
