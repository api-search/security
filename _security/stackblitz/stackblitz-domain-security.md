---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stackblitz.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: webcontainers.io
  spf: false
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: stackblitz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 05:13:41 2026 GMT
  host: developer.stackblitz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 01:13:50 2026 GMT
  host: webcontainers.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stackblitz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StackBlitz, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: StackBlitz
provider_slug: stackblitz
slug: stackblitz-domain-security
source_filename: stackblitz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stackblitz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\n- host: developer.stackblitz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:13:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: webcontainers.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 01:13:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stackblitz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: webcontainers.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackblitz/refs/heads/main/security/stackblitz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Developer Tools
- WebAssembly
- Node.js
- IDE
- Browser Runtime
- Code Environments
---
