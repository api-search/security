---
api_key_in: []
api_specs:
- filename: optum-dental-attachment-api-openapi.yml
  format: yaml
  label: Optum Medical Network Eligibility and Claims API
  slug: optum-medical-network-eligibility-and-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-dental-attachment-api-openapi.yml
- filename: optum-attachment-openapi.yml
  format: yaml
  label: Optum Real (Medical) API
  slug: optum-real-medical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-attachment-openapi.yml
- filename: optum-dental-pre-care-estimate-api-openapi.yml
  format: yaml
  label: Optum Real for Dental API
  slug: optum-real-for-dental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-dental-pre-care-estimate-api-openapi.yml
- filename: optum-formatting-rule-api-openapi.yml
  format: yaml
  label: Optum Pharmacy Solutions API
  slug: optum-pharmacy-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-formatting-rule-api-openapi.yml
- filename: optum-edi-enrollment-v1-openapi.yml
  format: yaml
  label: Optum Payment and Reimbursement API
  slug: optum-payment-and-reimbursement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-edi-enrollment-v1-openapi.yml
- filename: optum-cms-common-facility-openapi.yml
  format: yaml
  label: Optum Insight Platform (Platform and Interoperability) API
  slug: optum-insight-platform-platform-and-interoperability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-cms-common-facility-openapi.yml
- filename: optum-abm-care-decision-support-api-openapi.yml
  format: yaml
  label: Optum Analytics and Insights API
  slug: optum-analytics-and-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-abm-care-decision-support-api-openapi.yml
- filename: optum-security-and-authorization-v2-openapi.yml
  format: yaml
  label: Optum API Tools — Security and Authorization
  slug: optum-api-tools-security-and-authorization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/openapi/optum-security-and-authorization-v2-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Optum Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Optum secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Optum
provider_slug: optum
scheme_count: 2
schemes:
- bearer_format: JWT
  credentials: client_id + client_secret provisioned during onboarding / sandbox access
  flows:
  - flow: clientCredentials
    token_url_production: https://apigw.optum.com/apip/auth/v2/token
    token_url_sandbox: https://sandbox-apigw.optum.com/apip/auth/v2/token
  name: OptumOAuth2 (Security and Authorization v2)
  notes: Consumers exchange client_id and client_secret for a short-lived (1 hour) JWT access_token returned with token_type "bearer" and expires_in 3600, then send it as a Bearer token over TLS 1.2+.
  request_header: 'Authorization: Bearer <access_token>'
  scheme: bearer
  spec: openapi/optum-security-and-authorization-v2-openapi.yml
  token_lifetime_seconds: 3600
  type: oauth2
  used_by:
  - Medical Network eligibility / claims / claim status / reports / attachments
  - Dental Attachment API
  - Enhanced Eligibility
  - Real Prior Authorization, Real Provider Access
- bearer_format: JWT
  flows:
  - flow: clientCredentials
    token_url_production: https://apigw.optum.com/apip/auth/sntl/v1/token
    token_url_sandbox: https://sandbox-apigw.optum.com/apip/auth/sntl/v1/token
  name: OptumOAuth2 (Security and Authorization v3 / sentinel)
  notes: The newer "sentinel" token endpoint. Both generations are live at the same time and the docs do not state a migration date, so a consumer must read the individual API's spec to know which token endpoint applies. That ambiguity is the single most consequential documentation gap on the platform.
  request_header: 'Authorization: Bearer <access_token>'
  scheme: bearer
  spec: openapi/optum-security-and-authorization-v3-openapi.yml
  type: oauth2
  used_by:
  - Optum Real oihub APIs (claim actions, claim inquiry, document search, benefit check, auth referral, pre-service eligibility)
  - Real Dental pre-care eligibility and claim status
slug: optum-authentication
source_filename: optum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://developer.optum.com/apitools/reference/security-and-authorization-v2-overview\ndocs:\n  - https://developer.optum.com/eligibilityandclaims/docs/optum-security-and-authorization\n  - https://developer.optum.com/apitools/reference/security-and-authorization-v2-overview\n  - https://developer.optum.com/apitools/reference/security-and-authorization-v3-overview\nderived_from: openapi/_original/*.json (25 oauth2 securitySchemes across 59 harvested documents)\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  api_key_in: []\n  transport_security: TLS 1.2+\n  scheme_count_in_specs: 50\n  scopes: [create_txn, read_txn, create_coveragediscovery, read_coveragediscovery, read_healthcheck]\n  note: >-\n    One mechanism, two generations. Every Optum API is protected by an OAuth2 client-credentials\n    bearer token; the only variation is which token endpoint issues it. A handful of the Optum Insight Platform\n\
  \    specs additionally declare a bare `http bearer` or `apiKey` scheme, but they resolve to the same\n    gateway token. There is no user-delegated authorization-code flow, no\n    mTLS and no basic auth anywhere in the public surface — which also means there is no\n    SMART-on-FHIR patient-authorization path on these endpoints.\nschemes:\n  - name: OptumOAuth2 (Security and Authorization v2)\n    type: oauth2\n    scheme: bearer\n    bearer_format: JWT\n    flows:\n      - flow: clientCredentials\n        token_url_production: https://apigw.optum.com/apip/auth/v2/token\n        token_url_sandbox: https://sandbox-apigw.optum.com/apip/auth/v2/token\n    token_lifetime_seconds: 3600\n    request_header: 'Authorization: Bearer <access_token>'\n    credentials: client_id + client_secret provisioned during onboarding / sandbox access\n    spec: openapi/optum-security-and-authorization-v2-openapi.yml\n    used_by:\n      - Medical Network eligibility / claims / claim status / reports / attachments\n\
  \      - Dental Attachment API\n      - Enhanced Eligibility\n      - Real Prior Authorization, Real Provider Access\n    notes: >-\n      Consumers exchange client_id and client_secret for a short-lived (1 hour) JWT access_token\n      returned with token_type \"bearer\" and expires_in 3600, then send it as a Bearer token over\n      TLS 1.2+.\n  - name: OptumOAuth2 (Security and Authorization v3 / sentinel)\n    type: oauth2\n    scheme: bearer\n    bearer_format: JWT\n    flows:\n      - flow: clientCredentials\n        token_url_production: https://apigw.optum.com/apip/auth/sntl/v1/token\n        token_url_sandbox: https://sandbox-apigw.optum.com/apip/auth/sntl/v1/token\n    request_header: 'Authorization: Bearer <access_token>'\n    spec: openapi/optum-security-and-authorization-v3-openapi.yml\n    used_by:\n      - Optum Real oihub APIs (claim actions, claim inquiry, document search, benefit check, auth referral, pre-service eligibility)\n      - Real Dental pre-care eligibility\
  \ and claim status\n    notes: >-\n      The newer \"sentinel\" token endpoint. Both generations are live at the same time and the docs\n      do not state a migration date, so a consumer must read the individual API's spec to know which\n      token endpoint applies. That ambiguity is the single most consequential documentation gap on\n      the platform.\nscopes_ref: scopes/optum-scopes.yml\nonboarding:\n  sandbox: https://marketplace.optum.com/apiservices/api-sandbox-access\n  production: 'Negotiated with an Optum representative; HIPAA data-use agreement and training required.'\nmfa_or_signing: none\nkey_rotation_documented: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optum/refs/heads/main/authentication/optum-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Healthcare
- Health Insurance
- Claims
- Eligibility
- FHIR
- Interoperability
- Pharmacy
- EDI
- X12
- Payments
- Prior Authorization
- Clearinghouse
- Revenue Cycle
- Dental
- Da Vinci
- Patient Access
- Remittance
- Attachments
- Payer Directory
---
