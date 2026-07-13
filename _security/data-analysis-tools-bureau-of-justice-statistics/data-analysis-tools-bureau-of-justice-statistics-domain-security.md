---
api_specs:
- filename: bjs-ncvs-api-openapi.yml
  format: yaml
  label: BJS NCVS API
  slug: ncvs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/data-analysis-tools-bureau-of-justice-statistics/refs/heads/main/openapi/bjs-ncvs-api-openapi.yml
- filename: bjs-nibrs-api-openapi.yml
  format: yaml
  label: BJS NIBRS National Estimates API
  slug: nibrs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/data-analysis-tools-bureau-of-justice-statistics/refs/heads/main/openapi/bjs-nibrs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ojp.gov
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: bjs.ojp.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: api.ojp.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Data Analysis Tools Bureau Of Justice Statistics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bureau of Justice Statistics Data Analysis Tools, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bureau of Justice Statistics Data Analysis Tools
provider_slug: data-analysis-tools-bureau-of-justice-statistics
slug: data-analysis-tools-bureau-of-justice-statistics-domain-security
source_filename: data-analysis-tools-bureau-of-justice-statistics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bjs.ojp.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ojp.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ojp.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-analysis-tools-bureau-of-justice-statistics/refs/heads/main/security/data-analysis-tools-bureau-of-justice-statistics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Crime Statistics
- Federal Government
- NCVS
- NIBRS
- Open Data
- SODA
- Statistics
- Victimization
---
