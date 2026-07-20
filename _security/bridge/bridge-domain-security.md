---
api_specs:
- filename: bridge-openapi-original.json
  format: json
  label: Bridge API
  slug: bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bridge/refs/heads/main/openapi/bridge-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 issue "ssl.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bridge.xyz
  spf: true
hosts:
- cert_expires: Sep 30 00:57:01 2026 GMT
  host: www.bridge.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: api.bridge.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bridge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bridge, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bridge
provider_slug: bridge
slug: bridge-domain-security
source_filename: bridge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bridge.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 00:57:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bridge.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bridge.xyz\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bridge/refs/heads/main/security/bridge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Stablecoins
- Payments
- Money Movement
- Cross-Border Payments
- Virtual Accounts
- Wallets
- Cards
- Fintech
---
