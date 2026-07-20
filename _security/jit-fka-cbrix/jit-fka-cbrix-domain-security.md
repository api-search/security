---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jit.io
  spf: true
hosts:
- cert_expires: Jan 17 23:59:59 2027 GMT
  host: www.jit.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 06:30:55 2026 GMT
  host: docs.jit.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: api.jit.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jit Fka Cbrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jit (fka Cbrix), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jit (fka Cbrix)
provider_slug: jit-fka-cbrix
slug: jit-fka-cbrix-domain-security
source_filename: jit-fka-cbrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.jit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:30:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.jit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: jit.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jit-fka-cbrix/refs/heads/main/security/jit-fka-cbrix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Application Security
- DevSecOps
- ASPM
- Security
- Vulnerability Management
- API
---
