---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getseam.ai
  spf: true
hosts:
- cert_expires: Oct 12 17:25:54 2026 GMT
  host: www.getseam.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Seam Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seam AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Seam AI
provider_slug: seam-ai
slug: seam-ai-domain-security
source_filename: seam-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getseam.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 17:25:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getseam.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seam-ai/refs/heads/main/security/seam-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Account Based Marketing
- Sales Intelligence
- Marketing
- AI Agents
- CRM
---
