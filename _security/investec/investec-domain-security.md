---
api_specs:
- filename: obie-account-info-openapi.yaml
  format: yaml
  label: Investec Account and Transaction Information API (AIS)
  slug: investec-account-transaction-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/investec/refs/heads/main/openapi/obie-account-info-openapi.yaml
- filename: obie-payment-initiation-openapi.yaml
  format: yaml
  label: Investec Payment Initiation API (PIS)
  slug: investec-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/investec/refs/heads/main/openapi/obie-payment-initiation-openapi.yaml
- filename: obie-confirmation-funds-openapi.yaml
  format: yaml
  label: Investec Confirmation of Funds API (CBPII)
  slug: investec-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/investec/refs/heads/main/openapi/obie-confirmation-funds-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: investec.com
  spf: true
hosts:
- cert_expires: Sep  9 10:24:12 2026 GMT
  host: www.investec.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 09:03:36 2026 GMT
  host: developer.investec.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: openapi.investec.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Investec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Investec, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Investec
provider_slug: investec
slug: investec-domain-security
source_filename: investec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.investec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 10:24:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.investec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 09:03:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: openapi.investec.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: investec.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/investec/refs/heads/main/security/investec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Specialist Bank
- Wealth Management
- FAPI
- Programmable Banking
---
