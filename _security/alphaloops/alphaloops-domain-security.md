---
api_specs:
- filename: alphaloops-carriers-api-openapi.yml
  format: yaml
  label: AlphaLoops FMCSA Carrier Data API Carriers API
  slug: alphaloops-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaloops/refs/heads/main/openapi/alphaloops-carriers-api-openapi.yml
- filename: alphaloops-contacts-api-openapi.yml
  format: yaml
  label: AlphaLoops FMCSA Carrier Data API Contacts API
  slug: alphaloops-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaloops/refs/heads/main/openapi/alphaloops-contacts-api-openapi.yml
- filename: alphaloops-inspections-api-openapi.yml
  format: yaml
  label: AlphaLoops FMCSA Carrier Data API Inspections API
  slug: alphaloops-inspections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaloops/refs/heads/main/openapi/alphaloops-inspections-api-openapi.yml
- filename: alphaloops-vins-api-openapi.yml
  format: yaml
  label: AlphaLoops FMCSA Carrier Data API Vins API
  slug: alphaloops-vins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alphaloops/refs/heads/main/openapi/alphaloops-vins-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: runalphaloops.com
  spf: false
hosts:
- cert_expires: Oct 30 07:04:40 2026 GMT
  host: runalphaloops.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 22:23:47 2026 GMT
  host: api.runalphaloops.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alphaloops Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AlphaLoops FMCSA Carrier Data API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: AlphaLoops FMCSA Carrier Data API
provider_slug: alphaloops
slug: alphaloops-domain-security
source_filename: alphaloops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runalphaloops.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 07:04:40 2026 GMT\n  hsts: false\n- host: api.runalphaloops.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 22:23:47 2026 GMT\n  hsts: null\ndomains:\n- domain: runalphaloops.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alphaloops/refs/heads/main/security/alphaloops-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- fmcsa api
- safer web api
- dot lookup
- carrier data
- Freight
- Trucking
- motor carrier
- fleet intelligence
- Sales Intelligence
- MCP Server
- Contact Enrichment
- Risk
- Fraud
---
