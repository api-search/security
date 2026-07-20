---
api_specs:
- filename: circuit-v1-openapi-original.json
  format: json
  label: Spoke Public API
  slug: spoke-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/openapi/circuit-v1-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spoke.com
  spf: true
hosts:
- cert_expires: Sep  9 03:23:44 2026 GMT
  host: spoke.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 01:38:55 2026 GMT
  host: developer.dispatch.spoke.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 09:24:19 2026 GMT
  host: api.spoke.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Circuit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Circuit, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Circuit
provider_slug: circuit
slug: circuit-domain-security
source_filename: circuit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spoke.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 03:23:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.dispatch.spoke.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 01:38:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.spoke.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 09:24:19 2026 GMT\n  hsts: null\ndomains:\n- domain: spoke.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circuit/refs/heads/main/security/circuit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Delivery
- Logistics
- Last Mile
- Route Optimization
- Dispatch
- Courier
- Fleet
- Proof of Delivery
- Field Service
---
