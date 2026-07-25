---
api_specs:
- filename: hampden-and-co-account-information-api-openapi.yml
  format: yaml
  label: Hampden & Co Account & Transaction Information API
  slug: hampden-and-co-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hampden-and-co/refs/heads/main/openapi/hampden-and-co-account-information-api-openapi.yml
- filename: hampden-and-co-payment-initiation-api-openapi.yml
  format: yaml
  label: Hampden & Co Payment Initiation API
  slug: hampden-and-co-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hampden-and-co/refs/heads/main/openapi/hampden-and-co-payment-initiation-api-openapi.yml
- filename: hampden-and-co-confirmation-of-funds-api-openapi.yml
  format: yaml
  label: Hampden & Co Confirmation of Funds API
  slug: hampden-and-co-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hampden-and-co/refs/heads/main/openapi/hampden-and-co-confirmation-of-funds-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hampdenbank.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hampdendigital.com
  spf: true
hosts:
- cert_expires: Oct 15 12:29:43 2026 GMT
  host: www.hampdenbank.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 23:59:59 2026 GMT
  host: developer-sandbox.hampdendigital.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hampden And Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hampden & Co, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hampden & Co
provider_slug: hampden-and-co
slug: hampden-and-co-domain-security
source_filename: hampden-and-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hampdenbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 12:29:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developer-sandbox.hampdendigital.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hampdenbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: hampdendigital.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hampden-and-co/refs/heads/main/security/hampden-and-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Private Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
---
