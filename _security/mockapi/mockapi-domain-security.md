---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mockapi.io
  spf: true
hosts:
- cert_expires: Aug 15 01:57:07 2026 GMT
  host: mockapi.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mockapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mockAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: mockAPI
provider_slug: mockapi
slug: mockapi-domain-security
source_filename: mockapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mockapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 01:57:07 2026 GMT\n  hsts: false\ndomains:\n- domain: mockapi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mockapi/refs/heads/main/security/mockapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Mocking
- CRUD
- Mock Server
- Mocking
- Platform
- Prototyping
- REST
- Testing
---
