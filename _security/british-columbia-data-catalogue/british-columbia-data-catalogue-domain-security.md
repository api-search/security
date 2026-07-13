---
api_specs:
- filename: british-columbia-data-catalogue-openapi.yml
  format: yaml
  label: BC Data Catalogue CKAN API
  slug: ckan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/british-columbia-data-catalogue/refs/heads/main/openapi/british-columbia-data-catalogue-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bc.ca
  spf: false
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: catalogue.data.gov.bc.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: British Columbia Data Catalogue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for British Columbia Data Catalogue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: British Columbia Data Catalogue
provider_slug: british-columbia-data-catalogue
slug: british-columbia-data-catalogue-domain-security
source_filename: british-columbia-data-catalogue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: catalogue.data.gov.bc.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bc.ca\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/british-columbia-data-catalogue/refs/heads/main/security/british-columbia-data-catalogue-domain-security.yml
summary_line: TLSv1.3
tags:
- Open Data
- Government
- Canadian Government
- British Columbia
- Provincial Data
- CKAN
- Geospatial
---
