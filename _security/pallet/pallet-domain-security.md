---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: pallet.com
  spf: true
hosts:
- cert_expires: Aug 22 02:43:25 2026 GMT
  host: www.pallet.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pallet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pallet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Pallet
provider_slug: pallet
slug: pallet-domain-security
source_filename: pallet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pallet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 02:43:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pallet.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pallet/refs/heads/main/security/pallet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Physical Ai
- Logistics
- Supply Chain
- Freight
- Transportation
- Artificial Intelligence
- Automation
---
