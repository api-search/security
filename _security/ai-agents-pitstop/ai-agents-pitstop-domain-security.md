---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ai-agents-pitstop.com
  spf: true
hosts:
- cert_expires: Jan  7 22:09:43 2027 GMT
  host: ai-agents-pitstop.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ai Agents Pitstop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Jungle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AI Jungle
provider_slug: ai-agents-pitstop
slug: ai-agents-pitstop-domain-security
source_filename: ai-agents-pitstop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai-agents-pitstop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 22:09:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ai-agents-pitstop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ai-agents-pitstop/refs/heads/main/security/ai-agents-pitstop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Workspace
- Professional-Services
- Automation
---
