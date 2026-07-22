---
api_specs:
- filename: uncovr-api-openapi-original.json
  format: json
  label: Uncovr API
  slug: uncovr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uncovr/refs/heads/main/openapi/uncovr-api-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: uncovr.ai
  spf: true
hosts:
- cert_expires: Sep  7 13:27:12 2026 GMT
  host: www.uncovr.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 11:14:57 2026 GMT
  host: api.uncovr.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uncovr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uncovr, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Uncovr
provider_slug: uncovr
slug: uncovr-domain-security
source_filename: uncovr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uncovr.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 13:27:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.uncovr.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 11:14:57 2026 GMT\n  hsts: null\ndomains:\n- domain: uncovr.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uncovr/refs/heads/main/security/uncovr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Healthcare
- Surgery
- Artificial Intelligence
- Computer Vision
- Medical Documentation
- Medical Billing
- Clinical Intelligence
---
