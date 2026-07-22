---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agileloop.ai
  spf: true
hosts:
- cert_expires: Sep 27 10:11:27 2026 GMT
  host: agileloop.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agile Loop Llc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agile Loop L.L.C., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agile Loop L.L.C.
provider_slug: agile-loop-llc
slug: agile-loop-llc-domain-security
source_filename: agile-loop-llc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agileloop.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 10:11:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agileloop.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agile-loop-llc/refs/heads/main/security/agile-loop-llc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Large Action Models
- LLM
- Automation
- Enterprise AI
- Foundation Models
---
