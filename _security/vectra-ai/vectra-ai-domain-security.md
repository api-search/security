---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vectra.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: vectra.io
  spf: false
hosts:
- cert_expires: Oct  2 15:47:38 2026 GMT
  host: www.vectra.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: support.vectra.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: api.vectra.io
  https: false
kind: domain-security
layout: security
method: probed
name: Vectra Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vectra AI, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vectra AI
provider_slug: vectra-ai
slug: vectra-ai-domain-security
source_filename: vectra-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vectra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:47:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.vectra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vectra.io\n  https: false\ndomains:\n- domain: vectra.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: vectra.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectra-ai/refs/heads/main/security/vectra-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cybersecurity
- NDR
- XDR
- AI Detection
- Network Security
- Cloud Security
- MXDR
---
