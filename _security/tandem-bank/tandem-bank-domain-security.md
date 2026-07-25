---
api_specs:
- filename: obie-standard-account-info-openapi.yaml
  format: yaml
  label: Tandem Bank Account and Transaction Information API (AIS)
  slug: tandem-bank-account-transaction-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tandem-bank/refs/heads/main/openapi/obie-standard-account-info-openapi.yaml
- filename: obie-standard-payment-initiation-openapi.yaml
  format: yaml
  label: Tandem Bank Payment Initiation API (PIS)
  slug: tandem-bank-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tandem-bank/refs/heads/main/openapi/obie-standard-payment-initiation-openapi.yaml
- filename: obie-standard-confirmation-funds-openapi.yaml
  format: yaml
  label: Tandem Bank Confirmation of Funds API (CBPII)
  slug: tandem-bank-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tandem-bank/refs/heads/main/openapi/obie-standard-confirmation-funds-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tandem.co.uk
  spf: true
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  - 0 iodef "mailto:security@token.io"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: token.io
  spf: true
hosts:
- cert_expires: Sep 18 20:48:12 2026 GMT
  host: www.tandem.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: developer.token.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tandem Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tandem Bank, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tandem Bank
provider_slug: tandem-bank
slug: tandem-bank-domain-security
source_filename: tandem-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tandem.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:48:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.token.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tandem.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: token.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 iodef \"mailto:security@token.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tandem-bank/refs/heads/main/security/tandem-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- Challenger Bank
- Fintech
---
