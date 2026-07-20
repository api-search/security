---
api_specs:
- filename: kondukto-aspm-openapi.yml
  format: yaml
  label: Invicti ASPM (Kondukto) REST API v2
  slug: aspm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/openapi/kondukto-aspm-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kondukto.io
  spf: true
hosts:
- cert_expires: Sep 23 22:10:03 2026 GMT
  host: kondukto.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 02:11:29 2026 GMT
  host: docs.kondukto.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.kondukto.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kondukto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kondukto, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kondukto
provider_slug: kondukto
slug: kondukto-domain-security
source_filename: kondukto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kondukto.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 22:10:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.kondukto.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 02:11:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.kondukto.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kondukto.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kondukto/refs/heads/main/security/kondukto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Application Security
- ASPM
- Vulnerability Management
- DevSecOps
- Security Orchestration
- SAST
- DAST
- SCA
- Software Composition Analysis
- Container Security
- SBOM
- Security Testing
- CI/CD
- Security
---
