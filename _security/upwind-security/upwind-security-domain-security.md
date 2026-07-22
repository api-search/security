---
api_specs:
- filename: upwind-security-management-v2-openapi.yml
  format: yaml
  label: Upwind Management REST API v2
  slug: management-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind-security/refs/heads/main/openapi/upwind-security-management-v2-openapi.yml
- filename: upwind-security-management-v1-openapi.yml
  format: yaml
  label: Upwind Management REST API v1
  slug: management-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind-security/refs/heads/main/openapi/upwind-security-management-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: upwind.io
  spf: true
hosts:
- cert_expires: Sep 15 05:11:08 2026 GMT
  host: www.upwind.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: docs.upwind.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.upwind.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upwind Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upwind Security, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Upwind Security
provider_slug: upwind-security
slug: upwind-security-domain-security
source_filename: upwind-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.upwind.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:11:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.upwind.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.upwind.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: upwind.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upwind-security/refs/heads/main/security/upwind-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Cloud Security
- CNAPP
- Runtime Security
- Vulnerability Management
- API Security
- Kubernetes
---
