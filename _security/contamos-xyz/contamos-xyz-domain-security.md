---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: contamos.xyz
  spf: true
hosts:
- cert_expires: Dec 21 18:07:11 2026 GMT
  host: contamos.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contamos Xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contamos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Contamos
provider_slug: contamos-xyz
slug: contamos-xyz-domain-security
source_filename: contamos-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contamos.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 18:07:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: contamos.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/contamos-xyz/security/contamos-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Ledger
- Multi-Currency
- AI Assistant
- Collaboration
---
