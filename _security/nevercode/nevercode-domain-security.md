---
api_specs:
- filename: nevercode-openapi-original.json
  format: json
  label: Codemagic REST API
  slug: codemagic-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/openapi/nevercode-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: codemagic.io
  spf: true
hosts:
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: codemagic.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: docs.codemagic.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nevercode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nevercode, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nevercode
provider_slug: nevercode
slug: nevercode-domain-security
source_filename: nevercode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codemagic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.codemagic.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: codemagic.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nevercode/refs/heads/main/security/nevercode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Continuous Integration
- Continuous Delivery
- CI/CD
- DevOps
- Mobile
- Flutter
- Builds
- App Distribution
- Code Signing
---
