---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vlt.io
  spf: true
hosts:
- cert_expires: Sep 29 00:10:36 2026 GMT
  host: www.vlt.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: registry.vlt.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vlt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for vlt, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: vlt
provider_slug: vlt
slug: vlt-domain-security
source_filename: vlt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vlt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 00:10:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: registry.vlt.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: vlt.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vlt/refs/heads/main/security/vlt-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- JavaScript
- Package Management
- Package Registry
- Developer Tools
- CLI
- Serverless
- npm
- Dependency Management
- Open Source
---
