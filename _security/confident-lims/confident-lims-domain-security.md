---
api_specs:
- filename: confident-lims-labs-openapi.json
  format: json
  label: Confident Cannabis API - Lab Endpoints
  slug: confident-cannabis-api-lab-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-labs-openapi.json
- filename: confident-lims-clients-openapi.json
  format: json
  label: Confident Cannabis API - Client Endpoints
  slug: confident-cannabis-api-client-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-clients-openapi.json
- filename: confident-lims-common-openapi.json
  format: json
  label: Confident Cannabis API - Common Reference Data
  slug: confident-cannabis-api-common-reference-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/openapi/confident-lims-common-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: confidentcannabis.com
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: api.confidentcannabis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Confident Lims Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Confident LIMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Confident LIMS
provider_slug: confident-lims
slug: confident-lims-domain-security
source_filename: confident-lims-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.confidentcannabis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: confidentcannabis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/confident-lims/refs/heads/main/security/confident-lims-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- LIMS
- Laboratory Information Management
- Analytical Testing
- Cannabis Testing
- Compliance
- Sample Management
- Lab Software
---
