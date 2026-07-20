---
api_specs:
- filename: archera-openapi-original.json
  format: json
  label: Archera Public API
  slug: archera-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/openapi/archera-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: archera.ai
  spf: true
hosts:
- cert_expires: Sep 23 23:11:03 2026 GMT
  host: archera.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 21:44:57 2026 GMT
  host: docs.archera.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.archera.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Archera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Archera, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Archera
provider_slug: archera
slug: archera-domain-security
source_filename: archera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: archera.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:11:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.archera.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 21:44:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.archera.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: archera.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/security/archera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- FinOps
- Cloud Cost Management
- Cloud Commitments
- Cost Optimization
- MCP
- Azure
- Google Cloud
---
