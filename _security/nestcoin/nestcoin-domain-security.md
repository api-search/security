---
api_specs:
- filename: nestcoin-external-gateway-openapi-original.json
  format: json
  label: Onboard External API Gateway
  slug: onboard-external-api-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nestcoin/refs/heads/main/openapi/nestcoin-external-gateway-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nestcoin.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: onboardpay.co
  spf: true
hosts:
- cert_expires: Oct 17 05:11:05 2026 GMT
  host: nestcoin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: external.dev.onboardpay.co
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nestcoin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nestcoin, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nestcoin
provider_slug: nestcoin
slug: nestcoin-domain-security
source_filename: nestcoin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nestcoin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 05:11:05 2026 GMT\n  hsts: false\n- host: external.dev.onboardpay.co\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nestcoin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: onboardpay.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nestcoin/refs/heads/main/security/nestcoin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Crypto
- Exchange
- On-Off Ramp
- Payments
- Web3
- Africa
---
