---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: classet.ai
  spf: true
hosts:
- cert_expires: Dec 15 16:44:26 2026 GMT
  host: www.classet.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Classet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Classet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Classet
provider_slug: classet
slug: classet-domain-security
source_filename: classet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.classet.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 16:44:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: classet.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/classet/refs/heads/main/security/classet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Recruiting
- ATS
- Automation
- Enterprise
---
