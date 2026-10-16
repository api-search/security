---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: controlrooms.ai
  spf: true
hosts:
- cert_expires: Nov 27 20:21:19 2026 GMT
  host: www.controlrooms.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Controlrooms Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ControlRooms.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ControlRooms.ai
provider_slug: controlrooms-ai
slug: controlrooms-ai-domain-security
source_filename: controlrooms-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.controlrooms.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 20:21:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: controlrooms.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/controlrooms-ai/refs/heads/main/security/controlrooms-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Anomaly Detection
- Plant Operations
- AI Troubleshooting
---
