---
api_specs:
- filename: centers-for-disease-control-and-prevention-openapi.yml
  format: yaml
  label: CDC Socrata Open Data API (data.cdc.gov)
  slug: cdc-socrata-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/openapi/centers-for-disease-control-and-prevention-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cdc.gov
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: www.cdc.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: open.cdc.gov
  https: false
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: data.cdc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Centers For Disease Control And Prevention Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Centers for Disease Control and Prevention, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Centers for Disease Control and Prevention
provider_slug: centers-for-disease-control-and-prevention
slug: centers-for-disease-control-and-prevention-domain-security
source_filename: centers-for-disease-control-and-prevention-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cdc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\n- host: open.cdc.gov\n  https: false\n- host: data.cdc.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cdc.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centers-for-disease-control-and-prevention/refs/heads/main/security/centers-for-disease-control-and-prevention-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CDC
- Environmental Health
- Epidemiology
- Federal Government
- Healthcare
- Open Data
- Public Health
- Socrata
- Surveillance
- WONDER
---
