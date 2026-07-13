---
api_specs:
- filename: celcoin-billissuance-settlement-openapi.json
  format: json
  label: Celcoin BaaS and Core Banking API
  slug: baas-core-banking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-billissuance-settlement-openapi.json
- filename: celcoin-credit-openapi.json
  format: json
  label: Celcoin Credit as a Service API
  slug: credit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/openapi/celcoin-credit-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: celcoin.com.br
  spf: true
hosts:
- cert_expires: Oct  8 15:00:37 2026 GMT
  host: www.celcoin.com.br
  hsts: true
  hsts_max_age: 10368000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 03:38:52 2026 GMT
  host: developers.celcoin.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:12:30 2026 GMT
  host: api.openfinance.celcoin.com.br
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Celcoin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celcoin, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Celcoin
provider_slug: celcoin
slug: celcoin-domain-security
source_filename: celcoin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.celcoin.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 15:00:37 2026 GMT\n  hsts: true\n  hsts_max_age: 10368000\n- host: developers.celcoin.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 03:38:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openfinance.celcoin.com.br\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 23:12:30 2026 GMT\n  hsts: null\ndomains:\n- domain: celcoin.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celcoin/refs/heads/main/security/celcoin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking as a Service
- BaaS
- Pix
- Boleto
- TED
- Bill Payments
- Prepaid Cards
- Digital Accounts
- Open Banking
- Open Finance
- Credit
- Fintech
- Brazil
- Financial Infrastructure
---
