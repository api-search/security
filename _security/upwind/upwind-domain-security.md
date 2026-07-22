---
api_specs:
- filename: upwind-management-v1-openapi.yml
  format: yaml
  label: Upwind Management REST API v1
  slug: upwind-management-rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-management-v1-openapi.yml
- filename: upwind-management-v2-openapi.yml
  format: yaml
  label: Upwind Management REST API v2
  slug: upwind-management-rest-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/openapi/upwind-management-v2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: upwind.io
  spf: true
hosts:
- cert_expires: Sep 15 21:02:27 2026 GMT
  host: upwind.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.upwind.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: api.eu.upwind.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Upwind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upwind, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Upwind
provider_slug: upwind
slug: upwind-domain-security
source_filename: upwind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upwind.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:02:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.upwind.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\n- host: api.eu.upwind.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: upwind.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upwind/refs/heads/main/security/upwind-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Cloud Security
- CNAPP
- Vulnerability Management
- Container Security
- Kubernetes
- API Security
- Threat Detection
- Data Security
---
