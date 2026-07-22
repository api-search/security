---
api_specs:
- filename: stablesea-openapi.json
  format: json
  label: Stable Sea Terminal API
  slug: stable-sea-terminal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stablesea/refs/heads/main/openapi/stablesea-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: stablesea.com
  spf: true
hosts:
- cert_expires: Aug 30 19:18:27 2026 GMT
  host: www.stablesea.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: api-sandbox.stablesea.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Stablesea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stablesea, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Stablesea
provider_slug: stablesea
slug: stablesea-domain-security
source_filename: stablesea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stablesea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 19:18:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-sandbox.stablesea.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: stablesea.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stablesea/refs/heads/main/security/stablesea-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Stablecoins
- Payments
- Cash Management
- Treasury
- Cross-Border Payments
- Liquidity
- Fintech
- On-Off Ramp
- Cryptocurrency
---
