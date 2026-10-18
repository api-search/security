---
api_specs:
- filename: gstinapi-bulk-api-openapi.yml
  format: yaml
  label: GSTIN API Bulk API
  slug: gstinapi-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gstinapi/refs/heads/main/openapi/gstinapi-bulk-api-openapi.yml
- filename: gstinapi-verification-api-openapi.yml
  format: yaml
  label: GSTIN API Verification API
  slug: gstinapi-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gstinapi/refs/heads/main/openapi/gstinapi-verification-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gstinapi.com
  spf: false
hosts:
- cert_expires: Nov 27 11:26:28 2026 GMT
  host: gstinapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gstinapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GSTIN API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: GSTIN API
provider_slug: gstinapi
slug: gstinapi-domain-security
source_filename: gstinapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gstinapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 11:26:28 2026 GMT\n  hsts: false\ndomains:\n- domain: gstinapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gstinapi/refs/heads/main/security/gstinapi-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- GST
- India
- Taxation
- API
---
