---
api_specs:
- filename: ppro-payment-charges-openapi.yml
  format: yaml
  label: PPRO Global API
  slug: ppro-global-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-payment-charges-openapi.yml
- filename: ppro-onboarding-openapi.yml
  format: yaml
  label: PPRO Onboarding API
  slug: ppro-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/openapi/ppro-onboarding-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: ppro.com
  spf: true
hosts:
- cert_expires: Nov 23 11:43:01 2026 GMT
  host: www.ppro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 12:49:55 2026 GMT
  host: developerhub.ppro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: api.eu.ppro.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ppro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PPRO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: PPRO
provider_slug: ppro
slug: ppro-domain-security
source_filename: ppro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ppro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 11:43:01 2026 GMT\n  hsts: null\n- host: developerhub.ppro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 12:49:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.eu.ppro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ppro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ppro/refs/heads/main/security/ppro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Local Payment Methods
- Financial Services
- Fintech
- Acquiring
- Checkout
- E-commerce
- Digital Wallets
- Recurring Payments
- Disputes
- Chargebacks
- Company
---
