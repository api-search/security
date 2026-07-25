---
api_key_in: []
auth_types:
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Handelsbanken Uk Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
- decoupled
overview: Handelsbanken UK secures its APIs with oauth2 and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials, authorizationCode, and decoupled flow(s).
provider_name: Handelsbanken UK
provider_slug: handelsbanken-uk
scheme_count: 4
schemes:
- description: Third-party providers authenticate the transport channel with a qualified certificate. Production requires a PSD2 eIDAS QWAC (Qualified Website Authentication Certificate) or a UK Open Banking OBWAC certificate issued by a Qualified Trust Service Provider (QTSP); QSEALC/OBSEAL is used for message signing. Sandbox access is available before certificate enrolment.
  name: TPP client authentication (mTLS)
  sources:
  - https://developer.handelsbanken.com/api/psd2/live
  type: mutualTLS
- description: Initial OAuth2 client-credentials token used for TPP client authentication against the gateway before a PSU consent/authorisation is obtained.
  flow: clientCredentials
  name: Client Credentials Grant
  sources:
  - https://developer.handelsbanken.com/api/psd2/guidelines
  type: oauth2
- description: Resulting from the Redirect Authorization (SCA) flow; the PSU authenticates at Handelsbanken and an authorization code is exchanged for an access token scoped to the consent or payment.
  flow: authorizationCode
  name: Authorization Code Grant (Redirect Authorization)
  sources:
  - https://developer.handelsbanken.com/api/psd2/guidelines
  type: oauth2
- description: Handelsbanken's non-standard decoupled SCA flow (the documented exception to the OAuth2 specification); the PSU approves out-of-band (e.g. banking app / BankID) and the TPP polls for the resulting token. Availability varies by country and by customer type (Individual vs Corporate).
  flow: decoupled
  name: Decoupled Grant (Decoupled Authorization)
  sources:
  - https://developer.handelsbanken.com/api/psd2/guidelines
  type: oauth2
slug: handelsbanken-uk-authentication
source_filename: handelsbanken-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.handelsbanken.com/api/psd2/guidelines\ndocs: https://developer.handelsbanken.com/api/psd2/guidelines\nnote: >-\n  Handelsbanken publishes no anonymously downloadable OpenAPI (the specs sit\n  behind portal login and the api.handelsbanken.com gateway rejects anonymous\n  TLS), so this profile is derived from the published PSD2 technical guidelines\n  rather than from a securitySchemes block. The APIs implement the Berlin Group\n  NextGenPSD2 authentication model.\nsummary:\n  types:\n  - oauth2\n  - mutualTLS\n  transport_security: mutual-TLS (mTLS)\n  oauth2_flows:\n  - clientCredentials\n  - authorizationCode\n  - decoupled\n  strong_customer_authentication: true\nschemes:\n- name: TPP client authentication (mTLS)\n  type: mutualTLS\n  description: >-\n    Third-party providers authenticate the transport channel with a qualified\n    certificate. Production requires a PSD2 eIDAS QWAC (Qualified Website\n\
  \    Authentication Certificate) or a UK Open Banking OBWAC certificate issued by\n    a Qualified Trust Service Provider (QTSP); QSEALC/OBSEAL is used for message\n    signing. Sandbox access is available before certificate enrolment.\n  sources:\n  - https://developer.handelsbanken.com/api/psd2/live\n- name: Client Credentials Grant\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Initial OAuth2 client-credentials token used for TPP client authentication\n    against the gateway before a PSU consent/authorisation is obtained.\n  sources:\n  - https://developer.handelsbanken.com/api/psd2/guidelines\n- name: Authorization Code Grant (Redirect Authorization)\n  type: oauth2\n  flow: authorizationCode\n  description: >-\n    Resulting from the Redirect Authorization (SCA) flow; the PSU authenticates\n    at Handelsbanken and an authorization code is exchanged for an access token\n    scoped to the consent or payment.\n  sources:\n  - https://developer.handelsbanken.com/api/psd2/guidelines\n\
  - name: Decoupled Grant (Decoupled Authorization)\n  type: oauth2\n  flow: decoupled\n  description: >-\n    Handelsbanken's non-standard decoupled SCA flow (the documented exception to\n    the OAuth2 specification); the PSU approves out-of-band (e.g. banking app /\n    BankID) and the TPP polls for the resulting token. Availability varies by\n    country and by customer type (Individual vs Corporate).\n  sources:\n  - https://developer.handelsbanken.com/api/psd2/guidelines\nconsent_model:\n  regulatory_consent: long-term consent applying across all AIS endpoints\n  short_term_consent: 15-minute consent (Sweden, individual users only)\n  identifiers:\n  - Consent-ID (AIS)\n  - Payment-ID (PIS)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/handelsbanken-uk/refs/heads/main/authentication/handelsbanken-uk-authentication.yml
summary_line: oauth2/mutualTLS · 4 schemes
tags:
- Banking
- Open Banking
- Financial Services
- PSD2
- Berlin Group
- NextGenPSD2
- Payments
- Account Information
- United Kingdom
- Fintech
---
