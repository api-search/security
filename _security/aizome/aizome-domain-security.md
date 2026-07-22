---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aizome.ai
  spf: true
hosts:
- cert_expires: Sep 10 11:17:39 2026 GMT
  host: aizome.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aizome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aizome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aizome
provider_slug: aizome
slug: aizome-domain-security
source_filename: aizome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aizome.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 11:17:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: aizome.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aizome/refs/heads/main/security/aizome-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- AI Agents
- Identity and Access
- Governance
- Compliance
- Agent Security
- Enterprise AI
---
