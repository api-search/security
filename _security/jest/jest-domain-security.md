---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jestjs.io
  spf: true
hosts:
- cert_expires: Sep 28 14:37:23 2026 GMT
  host: jestjs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Jest
provider_slug: jest
slug: jest-domain-security
source_filename: jest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jestjs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:37:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jestjs.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jest/refs/heads/main/security/jest-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- JavaScript
- Mocking
- Snapshot Testing
- Testing
- Unit Testing
---
