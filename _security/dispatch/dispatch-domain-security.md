---
api_specs:
- filename: dispatch-rest-v3-openapi.yml
  format: yaml
  label: Dispatch REST API v3
  slug: rest-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/openapi/dispatch-rest-v3-openapi.yml
- filename: dispatch-files-v1-openapi.yml
  format: yaml
  label: Dispatch Files API v1
  slug: files-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/openapi/dispatch-files-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dispatch.me
  spf: true
hosts:
- cert_expires: Oct  2 17:28:00 2026 GMT
  host: dispatch.me
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.dispatch.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: files-api.dispatch.me
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dispatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dispatch, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dispatch
provider_slug: dispatch
slug: dispatch-domain-security
source_filename: dispatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dispatch.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 17:28:00 2026 GMT\n  hsts: false\n- host: api.dispatch.me\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: files-api.dispatch.me\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dispatch.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dispatch/refs/heads/main/security/dispatch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Field Service
- Service Orchestration
- Work Orders
- Scheduling
- Contractor Networks
- Home Services
- Warranty
- Customer Experience
- Logistics
- Company
---
