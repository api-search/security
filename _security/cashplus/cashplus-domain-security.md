---
api_specs:
- filename: cashplus-account-information-openapi.yml
  format: yaml
  label: Cashplus Account Information API
  slug: cashplus-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashplus/refs/heads/main/openapi/cashplus-account-information-openapi.yml
- filename: cashplus-payment-initiation-openapi.yml
  format: yaml
  label: Cashplus Payment Initiation API
  slug: cashplus-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashplus/refs/heads/main/openapi/cashplus-payment-initiation-openapi.yml
- filename: cashplus-confirmation-of-funds-openapi.yml
  format: yaml
  label: Cashplus Confirmation of Funds API
  slug: cashplus-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cashplus/refs/heads/main/openapi/cashplus-confirmation-of-funds-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: zemplerbank.com
  spf: true
hosts:
- cert_expires: Sep 17 03:35:07 2026 GMT
  host: www.zemplerbank.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 15:33:51 2026 GMT
  host: developer.zemplerbank.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cashplus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cashplus Bank, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cashplus Bank
provider_slug: cashplus
slug: cashplus-domain-security
source_filename: cashplus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zemplerbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 03:35:07 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: developer.zemplerbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 15:33:51 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: zemplerbank.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cashplus/refs/heads/main/security/cashplus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- Challenger Bank
- Business Banking
- Fintech
---
