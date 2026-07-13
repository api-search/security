---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: testcontainers.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: testcontainers.cloud
  spf: true
hosts:
- cert_expires: Sep 29 02:53:48 2026 GMT
  host: testcontainers.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 20:26:30 2026 GMT
  host: app.testcontainers.cloud
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Testcontainers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Testcontainers, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Testcontainers
provider_slug: testcontainers
slug: testcontainers-domain-security
source_filename: testcontainers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: testcontainers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 02:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.testcontainers.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 20:26:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: testcontainers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: testcontainers.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testcontainers/refs/heads/main/security/testcontainers-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Testing
- Integration Testing
- Docker
- Containers
- CI/CD
- Developer Tools
---
