---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pnpm.io
  spf: true
hosts:
- cert_expires: Sep 22 05:53:18 2026 GMT
  host: pnpm.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pnpm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pnpm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: pnpm
provider_slug: pnpm
slug: pnpm-domain-security
source_filename: pnpm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pnpm.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 05:53:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pnpm.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pnpm/refs/heads/main/security/pnpm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Node.js
- Package Manager
- Monorepo
- JavaScript
- Open Source
- Developer Tools
- Dependency Management
- CLI
---
