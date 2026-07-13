---
api_specs:
- filename: isometric-registry-api-openapi.json
  format: json
  label: Isometric Registry API
  slug: isometric-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isometric/refs/heads/main/openapi/isometric-registry-api-openapi.json
- filename: isometric-certify-api-openapi.json
  format: json
  label: Isometric Certify Data Ingestion API
  slug: isometric-certify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/isometric/refs/heads/main/openapi/isometric-certify-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: isometric.com
  spf: true
hosts:
- cert_expires: Sep 20 22:51:04 2026 GMT
  host: isometric.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 09:35:52 2026 GMT
  host: docs.isometric.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 08:39:43 2026 GMT
  host: api.isometric.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Isometric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Isometric, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Isometric
provider_slug: isometric
slug: isometric-domain-security
source_filename: isometric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: isometric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 22:51:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.isometric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 09:35:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.isometric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 08:39:43 2026 GMT\n  hsts: null\ndomains:\n- domain: isometric.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isometric/refs/heads/main/security/isometric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Carbon Removal
- Carbon Registry
- Climate
- Climate Tech
- CDR
- MRV
- Measurement Reporting Verification
- Certification
- Superpollutants
- Biochar
- Direct Air Capture
- Enhanced Weathering
- Mineralization
- Reforestation
- Mangrove Restoration
- Agroforestry
- Methane
- HFC
- Sustainability
- ESG
- Net Zero
- LCA
- Greenhouse Gas
- Protocols
- AI
- MCP
---
