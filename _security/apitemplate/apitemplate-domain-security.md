---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apitemplate.io
  spf: true
hosts:
- cert_expires: Sep 27 02:11:29 2026 GMT
  host: apitemplate.io
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 02:11:29 2026 GMT
  host: rest.apitemplate.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apitemplate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APITemplate.io, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: APITemplate.io
provider_slug: apitemplate
slug: apitemplate-domain-security
source_filename: apitemplate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apitemplate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 02:11:29 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: rest.apitemplate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 02:11:29 2026 GMT\n  hsts: null\ndomains:\n- domain: apitemplate.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apitemplate/refs/heads/main/security/apitemplate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Generation
- PDF
- Images
- Templates
- API
- Jinja2
---
