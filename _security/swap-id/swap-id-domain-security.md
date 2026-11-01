---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swap.id
  spf: true
hosts:
- cert_expires: Jan 21 21:08:22 2027 GMT
  host: swap.id
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Swap Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for swap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: swap
provider_slug: swap-id
slug: swap-id-domain-security
source_filename: swap-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: swap.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 21:08:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: swap.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/swap-id/security/swap-id-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Mobility
- Battery
- Infrastructure
- IoT
---
