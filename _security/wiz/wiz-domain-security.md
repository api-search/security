---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: wiz.io
  spf: true
hosts:
- cert_expires: Sep 26 12:11:46 2026 GMT
  host: www.wiz.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 19:20:39 2026 GMT
  host: docs.wiz.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: api.us1.app.wiz.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wiz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wiz, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Wiz
provider_slug: wiz
slug: wiz-domain-security
source_filename: wiz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wiz.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 12:11:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.wiz.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 19:20:39 2026 GMT\n  hsts: null\n- host: api.us1.app.wiz.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wiz.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wiz/refs/heads/main/security/wiz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud Security
- CNAPP
- CSPM
- Vulnerability Management
- Cloud Native
- DevSecOps
- Security
---
