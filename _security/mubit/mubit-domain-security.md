---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mubit.co
  spf: true
hosts:
- cert_expires: Oct 19 21:35:11 2026 GMT
  host: mubit.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mubit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mubit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mubit
provider_slug: mubit
slug: mubit-domain-security
source_filename: mubit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mubit.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 21:35:11 2026 GMT\n  hsts: false\ndomains:\n- domain: mubit.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mubit/refs/heads/main/security/mubit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Storage
- Self Storage
- Logistics
- Warehousing
- Inventory Management
- Moving
- Mexico
---
