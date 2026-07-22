---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dylibso.ai
  spf: true
hosts:
- cert_expires: Sep 29 20:14:52 2026 GMT
  host: dylibso.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dylibso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dylibso, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dylibso
provider_slug: dylibso
slug: dylibso-domain-security
source_filename: dylibso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dylibso.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:14:52 2026 GMT\n  hsts: false\ndomains:\n- domain: dylibso.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dylibso/refs/heads/main/security/dylibso-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- WebAssembly
- Wasm
- Extensibility
- Plug-ins
- Developer Tools
- SDKs
- Model Context Protocol
- Open Source
- AI
---
