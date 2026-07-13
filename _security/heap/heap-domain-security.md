---
api_specs:
- filename: heap-openapi.yml
  format: yaml
  label: Heap Server-Side API
  slug: server-side-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heap/refs/heads/main/openapi/heap-openapi.yml
- filename: heap-webhooks-openapi.yml
  format: yaml
  label: Heap Partner Webhooks (Data-out API)
  slug: partner-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heap/refs/heads/main/openapi/heap-webhooks-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: heap.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: heapanalytics.com
  spf: true
hosts:
- cert_expires: Sep 28 15:44:11 2026 GMT
  host: www.heap.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 03:17:25 2026 GMT
  host: developers.heap.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: heapanalytics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heap, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Heap
provider_slug: heap
slug: heap-domain-security
source_filename: heap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heap.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 15:44:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.heap.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 03:17:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: heapanalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heap.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: heapanalytics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heap/refs/heads/main/security/heap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Autocapture
- Digital Analytics
- Product Analytics
- Session Replay
- User Behavior
---
