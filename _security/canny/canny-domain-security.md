---
api_specs:
- filename: canny-openapi.yml
  format: yaml
  label: Canny REST API
  slug: v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/openapi/canny-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: canny.io
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: canny.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: developers.canny.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Canny Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Canny, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Canny
provider_slug: canny
slug: canny-domain-security
source_filename: canny-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: canny.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.canny.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: canny.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/canny/refs/heads/main/security/canny-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Feedback
- Product Management
- Feature Requests
- Roadmap
- Changelog
- Voice of Customer
- SaaS
---
