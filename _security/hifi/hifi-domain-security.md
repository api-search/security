---
api_specs:
- filename: hifi-openapi-original.json
  format: json
  label: Hifi API
  slug: hifi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/openapi/hifi-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hifi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hifibridge.com
  spf: true
hosts:
- cert_expires: Sep 30 13:59:03 2026 GMT
  host: hifi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 02:20:51 2026 GMT
  host: docs.hifi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 12:13:07 2026 GMT
  host: production.hifibridge.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hifi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hifi, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hifi
provider_slug: hifi
slug: hifi-domain-security
source_filename: hifi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hifi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:59:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.hifi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 02:20:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: production.hifibridge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 12:13:07 2026 GMT\n  hsts: null\ndomains:\n- domain: hifi.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: hifibridge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hifi/refs/heads/main/security/hifi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Stablecoins
- Payments
- Money Movement
- On-Ramp
- Off-Ramp
- Crypto
- Fintech
- KYC
- Virtual Accounts
- Cross-Chain
- Financial Infrastructure
---
