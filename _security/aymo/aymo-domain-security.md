---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aymo.ai
  spf: true
hosts:
- cert_expires: Nov 20 04:11:32 2026 GMT
  host: aymo.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aymo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pimjo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pimjo
provider_slug: aymo
slug: aymo-domain-security
source_filename: aymo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aymo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 04:11:32 2026 GMT\n  hsts: false\ndomains:\n- domain: aymo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aymo/refs/heads/main/security/aymo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Platform
- Team Collaboration
- LLM
- Software-as-a-Service
---
