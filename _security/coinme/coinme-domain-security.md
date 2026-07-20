---
api_specs:
- filename: coinme-caas-openapi.json
  format: json
  label: Coinme Crypto-as-a-Service API
  slug: coinme-crypto-as-a-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinme/refs/heads/main/openapi/coinme-caas-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coinme.com
  spf: true
hosts:
- cert_expires: Sep 16 06:36:03 2026 GMT
  host: coinme.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 06:36:03 2026 GMT
  host: caas.coinme.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 06:36:03 2026 GMT
  host: caas-staging.coinme.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coinme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coinme, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coinme
provider_slug: coinme
slug: coinme-domain-security
source_filename: coinme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coinme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:36:03 2026 GMT\n  hsts: false\n- host: caas.coinme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:36:03 2026 GMT\n  hsts: null\n- host: caas-staging.coinme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:36:03 2026 GMT\n  hsts: null\ndomains:\n- domain: coinme.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinme/refs/heads/main/security/coinme-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- Cryptocurrency
- Payments
- Bitcoin
- Wallet
- KYC
- Onboarding
- Fintech
- Crypto-as-a-Service
- On-Ramp
- Off-Ramp
---
