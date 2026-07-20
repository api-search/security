---
api_specs:
- filename: confident-cannabis-lab-openapi.json
  format: json
  label: Confident Cannabis API - Lab Endpoints
  slug: confident-cannabis-api-lab-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-cannabis/refs/heads/main/openapi/confident-cannabis-lab-openapi.json
- filename: confident-cannabis-client-openapi.json
  format: json
  label: Confident Cannabis API - Client Endpoints
  slug: confident-cannabis-api-client-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-cannabis/refs/heads/main/openapi/confident-cannabis-client-openapi.json
- filename: confident-cannabis-common-openapi.json
  format: json
  label: Confident Cannabis API - Common Reference Data
  slug: confident-cannabis-api-common-reference-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-cannabis/refs/heads/main/openapi/confident-cannabis-common-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: confidentcannabis.com
  spf: true
hosts:
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: confidentcannabis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: api.confidentcannabis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Confident Cannabis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Confident Cannabis, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Confident Cannabis
provider_slug: confident-cannabis
slug: confident-cannabis-domain-security
source_filename: confident-cannabis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: confidentcannabis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.confidentcannabis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: confidentcannabis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confident-cannabis/refs/heads/main/security/confident-cannabis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cannabis
- Laboratory
- LIMS
- Testing
- Compliance
- Certificate of Analysis
- Life Sciences
---
