---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wasp.sh
  spf: false
hosts:
- cert_expires: Oct 18 04:34:24 2026 GMT
  host: wasp.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wasp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wasp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Wasp
provider_slug: wasp
slug: wasp-domain-security
source_filename: wasp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wasp.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 04:34:24 2026 GMT\n  hsts: false\ndomains:\n- domain: wasp.sh\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wasp/refs/heads/main/security/wasp-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Ai Enterprise Software
- Web Framework
- Full Stack
- Developer Tools
- React
- Node.js
- TypeScript
- Open Source
- AI Coding
---
