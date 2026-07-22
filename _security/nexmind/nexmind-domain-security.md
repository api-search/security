---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nexlaw.ai
  spf: true
hosts:
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: nexlaw.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexmind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NexMind, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NexMind
provider_slug: nexmind
slug: nexmind-domain-security
source_filename: nexmind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nexlaw.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nexlaw.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexmind/refs/heads/main/security/nexmind-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Legal
- Legal AI
- Legal Research
- Artificial Intelligence
- Litigation
- Document Analysis
- SaaS
---
