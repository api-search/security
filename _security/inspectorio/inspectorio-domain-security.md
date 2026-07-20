---
api_specs:
- filename: inspectorio-qrm-openapi.json
  format: json
  label: Inspectorio Quality Risk Management API
  slug: inspectorio-quality-risk-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inspectorio/refs/heads/main/openapi/inspectorio-qrm-openapi.json
- filename: inspectorio-rsc-openapi.json
  format: json
  label: Inspectorio Responsible Sourcing & Compliance API
  slug: inspectorio-responsible-sourcing-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inspectorio/refs/heads/main/openapi/inspectorio-rsc-openapi.json
- filename: inspectorio-fms-openapi.json
  format: json
  label: Inspectorio File Management API
  slug: inspectorio-file-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inspectorio/refs/heads/main/openapi/inspectorio-fms-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inspectorio.com
  spf: true
hosts:
- cert_expires: Oct  5 18:52:58 2026 GMT
  host: inspectorio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 13:59:25 2026 GMT
  host: files-integration.inspectorio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 00:20:36 2026 GMT
  host: files-integration.pre.inspectorio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inspectorio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inspectorio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Inspectorio
provider_slug: inspectorio
slug: inspectorio-domain-security
source_filename: inspectorio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inspectorio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 18:52:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: files-integration.inspectorio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 13:59:25 2026 GMT\n  hsts: null\n- host: files-integration.pre.inspectorio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 00:20:36 2026 GMT\n  hsts: null\ndomains:\n- domain: inspectorio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inspectorio/refs/heads/main/security/inspectorio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Supply Chain
- Quality Management
- Compliance
- Responsible Sourcing
- Traceability
- Manufacturing
- Retail
- Lab Testing
- Company
---
