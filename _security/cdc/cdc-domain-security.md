---
api_specs:
- filename: docs
  format: yaml
  label: CDC Open Data API
  slug: cdc-open-data-api
  spec_type: OpenAPI
  url: https://data.cdc.gov/api/docs
- filename: dibbs-ecr-refiner-openapi.json
  format: json
  label: DIBBs eCR Refiner API
  slug: dibbs-ecr-refiner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdc/refs/heads/main/openapi/dibbs-ecr-refiner-openapi.json
- filename: dibbs-query-connector-openapi.yaml
  format: yaml
  label: DIBBs Query Connector API
  slug: dibbs-query-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cdc/refs/heads/main/openapi/dibbs-query-connector-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cdc.gov
  spf: true
hosts:
- host: open.cdc.gov
  https: false
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: data.cdc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 28 13:32:05 2026 GMT
  host: wonder.cdc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cdc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CDC, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CDC
provider_slug: cdc
slug: cdc-domain-security
source_filename: cdc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open.cdc.gov\n  https: false\n- host: data.cdc.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wonder.cdc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:32:05 2026 GMT\n  hsts: null\ndomains:\n- domain: cdc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdc/refs/heads/main/security/cdc-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Public Health
- Disease Surveillance
- Vaccination
- Health Statistics
- Government
- Open Data
- Environmental Health
- Mortality
- CDC WONDER
---
