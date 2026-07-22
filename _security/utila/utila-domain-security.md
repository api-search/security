---
api_specs:
- filename: utila-v2-openapi-original.json
  format: json
  label: Utila API v2
  slug: utila-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utila/refs/heads/main/openapi/utila-v2-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: utila.io
  spf: true
hosts:
- cert_expires: Sep 30 15:02:41 2026 GMT
  host: utila.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 04:18:27 2026 GMT
  host: api.utila.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Utila Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Utila, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Utila
provider_slug: utila
slug: utila-domain-security
source_filename: utila-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: utila.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:02:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.utila.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 04:18:27 2026 GMT\n  hsts: null\ndomains:\n- domain: utila.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utila/refs/heads/main/security/utila-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Web3
- Digital Assets
- Stablecoins
- Custody
- MPC Wallets
- Blockchain
- Payments
- Treasury
---
