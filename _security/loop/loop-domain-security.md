---
api_specs:
- filename: loop-openapi-original.json
  format: json
  label: Loop API
  slug: loop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-openapi-original.json
- filename: loop-onboarding-openapi-original.json
  format: json
  label: Loop Onboarding API
  slug: loop-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/openapi/loop-onboarding-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: loop.com
  spf: true
hosts:
- cert_expires: Sep 12 20:47:11 2026 GMT
  host: loop.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 22:50:38 2026 GMT
  host: docs.loop.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: api.loop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loop, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Loop
provider_slug: loop
slug: loop-domain-security
source_filename: loop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 20:47:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.loop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 22:50:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.loop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: loop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loop/refs/heads/main/security/loop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Supply Chain
- Freight
- Freight Audit
- Payments
- Transportation
- Artificial Intelligence
- Data Platform
---
