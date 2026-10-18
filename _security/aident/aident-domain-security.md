---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aident.ai
  spf: true
hosts:
- cert_expires: Jan  3 06:02:01 2027 GMT
  host: aident.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aident Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aident Loadout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aident Loadout
provider_slug: aident
slug: aident-domain-security
source_filename: aident-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aident.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 06:02:01 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aident.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aident/refs/heads/main/security/aident-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Integration
- Automation
- Platform
---
