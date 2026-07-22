---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: simular.ai
  spf: true
hosts:
- cert_expires: Sep 11 23:30:11 2026 GMT
  host: simular.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simular Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simular, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Simular
provider_slug: simular
slug: simular-domain-security
source_filename: simular-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts\nhosts:\n- host: simular.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:30:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: simular.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simular/refs/heads/main/security/simular-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Computer Use
- Browser Automation
- Desktop Automation
- Agentic
- SDK
- Developer Tools
- Open Source
---
