---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bolt.new
  spf: true
hosts:
- cert_expires: Oct  6 03:55:23 2026 GMT
  host: bolt.new
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bolt New Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bolt.new, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bolt.new
provider_slug: bolt-new
slug: bolt-new-domain-security
source_filename: bolt-new-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bolt.new\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:55:23 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: bolt.new\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bolt-new/refs/heads/main/security/bolt-new-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- AI App Builder
- No-Code
- Low-Code
- Full-Stack
- WebContainers
- In-Browser IDE
- WebAssembly
- Node.js
- StackBlitz
- Generative UI
- Vibe Coding
- Agent
- Netlify
- Supabase
---
