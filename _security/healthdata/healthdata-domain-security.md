---
api_specs:
- filename: endpoints.html
  format: yaml
  label: HealthData.gov SODA API
  slug: healthdatagov-soda-api
  spec_type: OpenAPI
  url: https://dev.socrata.com/docs/endpoints.html
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: healthdata.gov
  spf: true
hosts:
- cert_expires: Mar 29 21:11:13 2027 GMT
  host: healthdata.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Healthdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HealthData.gov, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: HealthData.gov
provider_slug: healthdata
slug: healthdata-domain-security
source_filename: healthdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: healthdata.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 29 21:11:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: healthdata.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healthdata/refs/heads/main/security/healthdata-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Health
- Open Data
- Federal Government
- Medicare
- Medicaid
- Hospital Quality
- Drug Utilization
- Public Health
- CDC
- CMS
- FDA
- NIH
- SODA
- Socrata
---
