---
api_specs:
- filename: heap-add-account-properties-api-openapi.yml
  format: yaml
  label: Heap Add Account Properties API
  slug: heap-add-account-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heap/refs/heads/main/openapi/heap-add-account-properties-api-openapi.yml
- filename: heap-add-user-properties-api-openapi.yml
  format: yaml
  label: Heap Add User Properties API
  slug: heap-add-user-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heap/refs/heads/main/openapi/heap-add-user-properties-api-openapi.yml
- filename: heap-identify-api-openapi.yml
  format: yaml
  label: Heap Identify API
  slug: heap-identify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heap/refs/heads/main/openapi/heap-identify-api-openapi.yml
- filename: heap-track-api-openapi.yml
  format: yaml
  label: Heap Track API
  slug: heap-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heap/refs/heads/main/openapi/heap-track-api-openapi.yml
- filename: heap-webhooks-api-openapi.yml
  format: yaml
  label: Heap Webhooks API
  slug: heap-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heap/refs/heads/main/openapi/heap-webhooks-api-openapi.yml
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
