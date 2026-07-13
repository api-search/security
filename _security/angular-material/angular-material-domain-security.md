---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: angular.dev
  spf: false
hosts:
- cert_expires: Sep 24 00:33:34 2026 GMT
  host: material.angular.dev
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Angular Material Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Angular Material, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Angular Material
provider_slug: angular-material
slug: angular-material-domain-security
source_filename: angular-material-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: material.angular.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 00:33:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: angular.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/angular-material/refs/heads/main/security/angular-material-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Accessibility
- Angular
- Frontend
- Material Design
- Material Design 3
- Open Source
- TypeScript
- UI Components
---
