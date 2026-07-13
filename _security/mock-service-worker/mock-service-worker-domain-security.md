---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: mswjs.io
  spf: false
hosts:
- cert_expires: Sep 19 23:54:38 2026 GMT
  host: mswjs.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mock Service Worker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mock Service Worker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Mock Service Worker
provider_slug: mock-service-worker
slug: mock-service-worker-domain-security
source_filename: mock-service-worker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mswjs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:54:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mswjs.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mock-service-worker/refs/heads/main/security/mock-service-worker-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API Mocking
- GraphQL
- HTTP
- Mock Server
- Mocking
- Service Worker
- Testing
- WebSocket
---
