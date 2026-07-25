---
api_key_in: []
api_specs:
- filename: downloads
  format: yaml
  label: SIX bLink API
  slug: blink-api
  spec_type: Postman
  url: https://docs.blink.six-group.com/docs/downloads
- filename: six-group-card-management-api-openapi.yml
  format: yaml
  label: SIX debiX API
  slug: debix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/six-group/refs/heads/main/openapi/six-group-card-management-api-openapi.yml
- filename: six-group-3ds-authentication-api-openapi.yml
  format: yaml
  label: SIX debiX Auth Provider API
  slug: debix-auth-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/six-group/refs/heads/main/openapi/six-group-3ds-authentication-api-openapi.yml
- filename: six-group-bankmaster-api-openapi.yml
  format: yaml
  label: Swiss Bank Master API
  slug: swiss-bank-master-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/six-group/refs/heads/main/openapi/six-group-bankmaster-api-openapi.yml
- filename: six-group-status-api-openapi.yml
  format: yaml
  label: SIC Service Status API
  slug: sic-service-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/six-group/refs/heads/main/openapi/six-group-status-api-openapi.yml
- filename: six-group-calendar-api-openapi.yml
  format: yaml
  label: SIC Clearing Day Calendar API
  slug: sic-clearing-day-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/six-group/refs/heads/main/openapi/six-group-calendar-api-openapi.yml
- filename: six-group-detailedsettlementinformation-api-openapi.yml
  format: yaml
  label: Settlement Info Reporting API
  slug: settlement-info-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/six-group/refs/heads/main/openapi/six-group-detailedsettlementinformation-api-openapi.yml
auth_types:
- mutualTLS
- oauth2
- none
description: ''
kind: authentication
layout: security
method: searched
name: Six Group Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: SIX secures its APIs with mutualTLS, oauth2, and none across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: SIX
provider_slug: six-group
scheme_count: 6
schemes:
- description: All bLink connections are mutually authenticated with X.509 client certificates over TLS 1.2+. Certificates must be OV or EV, RSA >= 3072 bits, sha224-512RSA signature, ~1 year validity, issued by an accepted CA (DigiCert, QuoVadis, SwissSign) and registered with SIX; the platform maps the certificate to a client_id used to match access tokens.
  docs: https://docs.blink.six-group.com/api-reference/authentication/tls-certificates
  name: mTLS client certificates (bLink)
  type: mutualTLS
- description: bLink consent management uses standard OAuth 2.0 authorization-code consent flows (including App2App/Web2App inter-app flows), with token issuance, revocation, and username validation endpoints in the consent-flow base module; Consent 2.0 (permissions) and Consent 3.0 (grant management) blueprints are documented. Access tokens are bound to the mTLS-registered client_id.
  docs: https://docs.blink.six-group.com/api-reference/authentication/consent-management
  name: OAuth 2.0 consent flows (bLink)
  type: oauth2
- description: debiX issuers provide separate client certificates for the test and production environments; SIX registers the certificate DN in the debiX Portal and issuers verify access via the /healthcheck endpoint across all verbs.
  docs: https://docs.debix.six-group.com/getting-started
  name: mTLS client certificates (debiX)
  type: mutualTLS
- description: The sales-gated SIX Web API and Bulk API for financial information use MTLS certificate authentication; onboarding and certificates are handled through the SIX API Portal after a demo-access request.
  docs: https://www.six-group.com/en/products-services/financial-information/delivery-methods/api/web.html
  name: mTLS client certificates (SIX Web API / Bulk API)
  type: mutualTLS
- description: Documented production endpoints of the Swiss Bank Master API and SIC Service Status API answered HTTP 200 without authentication (probed 2026-07-21/22).
  name: Unauthenticated public endpoints
  type: none
- description: The Kong developer portal itself publishes RFC 8414 metadata (authorization_code + PKCE S256) for portal login - captured in well-known/six-group-oauth-authorization-server.json; this governs portal access, not product API calls.
  docs: https://apiportal.six-group.com/.well-known/oauth-authorization-server
  name: Developer-portal login OAuth (apiportal.six-group.com)
  type: oauth2
slug: six-group-authentication
source_filename: six-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://docs.blink.six-group.com/api-reference/authentication/tls-certificates.md\ndocs:\n- https://docs.blink.six-group.com/api-reference/authentication/tls-certificates\n- https://docs.blink.six-group.com/api-reference/authentication/consent-management\n- https://docs.debix.six-group.com/getting-started\n- https://www.six-group.com/en/products-services/financial-information/delivery-methods/api/web.html\nnote: None of the published OpenAPI documents declare securitySchemes - authentication\n  across the SIX API estate is transport-level mutual TLS, documented in prose, plus\n  OAuth 2.0 consent flows on bLink. Four Swiss infrastructure APIs on the shared\n  catalog (Swiss Bank Master, SIC Service Status, SIC Clearing Day Calendar,\n  Settlement Info Reporting healthcheck surface) respond without authentication.\nsummary:\n  types: [mutualTLS, oauth2, none]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: mTLS client\
  \ certificates (bLink)\n  type: mutualTLS\n  description: All bLink connections are mutually authenticated with X.509 client\n    certificates over TLS 1.2+. Certificates must be OV or EV, RSA >= 3072 bits,\n    sha224-512RSA signature, ~1 year validity, issued by an accepted CA (DigiCert,\n    QuoVadis, SwissSign) and registered with SIX; the platform maps the certificate\n    to a client_id used to match access tokens.\n  docs: https://docs.blink.six-group.com/api-reference/authentication/tls-certificates\n- name: OAuth 2.0 consent flows (bLink)\n  type: oauth2\n  description: bLink consent management uses standard OAuth 2.0 authorization-code\n    consent flows (including App2App/Web2App inter-app flows), with token issuance,\n    revocation, and username validation endpoints in the consent-flow base module;\n    Consent 2.0 (permissions) and Consent 3.0 (grant management) blueprints are\n    documented. Access tokens are bound to the mTLS-registered client_id.\n  docs: https://docs.blink.six-group.com/api-reference/authentication/consent-management\n\
  - name: mTLS client certificates (debiX)\n  type: mutualTLS\n  description: debiX issuers provide separate client certificates for the test and\n    production environments; SIX registers the certificate DN in the debiX Portal\n    and issuers verify access via the /healthcheck endpoint across all verbs.\n  docs: https://docs.debix.six-group.com/getting-started\n- name: mTLS client certificates (SIX Web API / Bulk API)\n  type: mutualTLS\n  description: The sales-gated SIX Web API and Bulk API for financial information\n    use MTLS certificate authentication; onboarding and certificates are handled\n    through the SIX API Portal after a demo-access request.\n  docs: https://www.six-group.com/en/products-services/financial-information/delivery-methods/api/web.html\n- name: Unauthenticated public endpoints\n  type: none\n  description: Documented production endpoints of the Swiss Bank Master API and SIC\n    Service Status API answered HTTP 200 without authentication (probed 2026-07-21/22).\n\
  - name: Developer-portal login OAuth (apiportal.six-group.com)\n  type: oauth2\n  description: The Kong developer portal itself publishes RFC 8414 metadata\n    (authorization_code + PKCE S256) for portal login - captured in\n    well-known/six-group-oauth-authorization-server.json; this governs portal\n    access, not product API calls.\n  docs: https://apiportal.six-group.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/six-group/refs/heads/main/authentication/six-group-authentication.yml
summary_line: mutualTLS/oauth2/none · 6 schemes
tags:
- Financial
- Market Data
- Stocks
- Reference Data
- Corporate Actions
- Real-Time
- Exchange
- Open Banking
- Payments
- Switzerland
---
