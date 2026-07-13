---
api_specs:
- filename: qlty-openapi.yml
  format: yaml
  label: Qlty CLI
  slug: qlty-cli
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlty/refs/heads/main/openapi/qlty-openapi.yml
- filename: qlty-openapi.yml
  format: yaml
  label: Qlty Coverage Upload
  slug: qlty-coverage-upload
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlty/refs/heads/main/openapi/qlty-openapi.yml
- filename: qlty-openapi.yml
  format: yaml
  label: Qlty Cloud API
  slug: qlty-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qlty/refs/heads/main/openapi/qlty-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qlty.sh
  spf: true
hosts:
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: qlty.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 00:09:49 2026 GMT
  host: docs.qlty.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qlty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qlty, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Qlty
provider_slug: qlty
slug: qlty-domain-security
source_filename: qlty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qlty.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.qlty.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 00:09:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: qlty.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qlty/refs/heads/main/security/qlty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Code Quality
- Code Coverage
- Static Analysis
- Linting
- Developer Tools
---
