---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Future Perfect Healthcare Authentication
name_suffix: Authentication
oauth_flows: []
overview: Future Perfect (Healthcare) declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Future Perfect (Healthcare)
provider_slug: future-perfect-healthcare
scheme_count: 3
schemes:
- description: '"Open security standards (OAuth2/OpenIdConnect) providing Single-Sign-On with the customer''s systems." Deployed as identity federation against the buying organisation''s existing identity provider.'
  flows: unpublished
  issuer: unpublished
  name: OAuth 2.0 / OpenID Connect single sign-on
  scopes_published: false
  source: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/557090777176539
  type: oauth2
- description: G-Cloud 14 "User authentication" field lists "Public key authentication (including by TLS client certificate)" among supported user authentication methods.
  name: Public key authentication including TLS client certificate
  source: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/557090777176539
  type: mutualTLS
- description: G-Cloud 14 "User authentication" field lists "2-factor authentication" and "Username or password". Management access authentication is declared as 2-factor; the web administration portal is additionally restricted to whitelisted IP addresses.
  name: Username and password with 2-factor authentication
  source: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/557090777176539
  type: http
slug: future-perfect-healthcare-authentication
source_filename: future-perfect-healthcare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/557090777176539\ndocs: null\nnote: >-\n  There is no public authentication reference and no securitySchemes block to derive from —\n  Future Perfect publishes no OpenAPI. Everything below is taken verbatim from the\n  supplier-authored identity/authentication fields of the G-Cloud 14 PANACEA service entry,\n  which is the only public description of how the platform authenticates. Scheme details\n  (token endpoints, issuer, scopes, header names) are NOT published anywhere public.\n\napi: PANACEA (no public base URL published)\npublic_reference: false\n\nschemes:\n- type: oauth2\n  name: OAuth 2.0 / OpenID Connect single sign-on\n  description: >-\n    \"Open security standards (OAuth2/OpenIdConnect) providing Single-Sign-On with the\n    customer's systems.\" Deployed as identity federation against the buying organisation's\n    existing identity provider.\n\
  \  flows: unpublished\n  issuer: unpublished\n  scopes_published: false\n  source: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/557090777176539\n- type: mutualTLS\n  name: Public key authentication including TLS client certificate\n  description: >-\n    G-Cloud 14 \"User authentication\" field lists \"Public key authentication (including by\n    TLS client certificate)\" among supported user authentication methods.\n  source: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/557090777176539\n- type: http\n  name: Username and password with 2-factor authentication\n  description: >-\n    G-Cloud 14 \"User authentication\" field lists \"2-factor authentication\" and \"Username or\n    password\". Management access authentication is declared as 2-factor; the web\n    administration portal is additionally restricted to whitelisted IP addresses.\n  source: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/557090777176539\n\
  \nidentity_federation: true\nmfa: true\nip_allowlisting:\n  present: true\n  scope: web administration portal\n  source: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/557090777176539\n\ntransport:\n  tls: 'TLS 1.2 or above between buyer and supplier networks and within the supplier network'\n  caveat: >-\n    The same G-Cloud field also declares \"Legacy SSL and TLS (under version 1.2)\" as a\n    supported data-in-transit protection option, alongside IPsec/TLS VPN gateway.\n  source: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/557090777176539\n\naudit:\n  user_audit: 'Users have access to real-time audit information; retention is user-defined.'\n  supplier_audit: 'Users contact the support team to get audit information.'\n  source: https://www.applytosupply.digitalmarketplace.service.gov.uk/g-cloud/services/557090777176539\n\ngaps:\n- No public OAuth metadata document (/.well-known/openid-configuration returned 404).\n- No\
  \ published scope or permission reference, so scopes/ is not written for this provider.\n- No public token endpoint, client registration flow, or key-issuance documentation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/future-perfect-healthcare/refs/heads/main/authentication/future-perfect-healthcare-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Healthcare
- Health IT
- Electronic Health Records
- openEHR
- Interoperability
- Clinical Decision Support
- Genomics
- Artificial Intelligence
- NHS
- United Kingdom
---
