---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: dropzone.ai
  spf: true
hosts:
- cert_expires: Sep 12 12:47:19 2026 GMT
  host: www.dropzone.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dropzone Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dropzone AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Dropzone AI
provider_slug: dropzone-ai
slug: dropzone-ai-domain-security
source_filename: dropzone-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dropzone.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 12:47:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dropzone.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dropzone-ai/refs/heads/main/security/dropzone-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- SOC
- AI Agent
- Autonomous
- Triage
- SIEM
- EDR
- XDR
- Gated
---
