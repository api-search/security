---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: glif.app
  spf: true
hosts:
- cert_expires: Sep 11 00:32:05 2026 GMT
  host: glif.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 10:43:07 2026 GMT
  host: docs.glif.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 03:04:04 2026 GMT
  host: simple-api.glif.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glif App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glif, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Glif
provider_slug: glif-app
slug: glif-app-domain-security
source_filename: glif-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glif.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 00:32:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.glif.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 10:43:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: simple-api.glif.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 03:04:04 2026 GMT\n  hsts: false\ndomains:\n- domain: glif.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glif-app/refs/heads/main/security/glif-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Artificial Intelligence
- No-Code
- Workflows
- Creative AI
- Generative AI
- Video Generation
- Image Generation
- ComfyUI
- MCP
- LLM Apps
---
