---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fin.tech
  spf: true
hosts:
- cert_expires: Sep  5 03:25:17 2026 GMT
  host: www.fin.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fintech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fintech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fintech
provider_slug: fintech
slug: fintech-domain-security
source_filename: fintech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fin.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 03:25:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fin.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fintech/refs/heads/main/security/fintech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Payments
- Stablecoins
- Banking
- Cross-Border Payments
- Settlement
- Fintech
---
