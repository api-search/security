---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: skan.ai
  spf: true
hosts:
- cert_expires: Sep 20 20:56:45 2026 GMT
  host: skan.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Skan
provider_slug: skan
slug: skan-domain-security
source_filename: skan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skan.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:56:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: skan.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skan/refs/heads/main/security/skan-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Process Intelligence
- Task Mining
- Process Mining
- AI Agents
- Enterprise Automation
- Workflow Intelligence
- Agentic AI
---
