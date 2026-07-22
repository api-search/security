---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: conifer.build
  spf: true
hosts:
- cert_expires: Oct 11 02:32:43 2026 GMT
  host: conifer.build
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conifer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conifer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Conifer
provider_slug: conifer
slug: conifer-domain-security
source_filename: conifer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conifer.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 02:32:43 2026 GMT\n  hsts: false\ndomains:\n- domain: conifer.build\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conifer/refs/heads/main/security/conifer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Local AI
- Inference
- Large Language Models
- Developer Tools
- Model Routing
- Desktop Application
- Privacy
- Rust
---
