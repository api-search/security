---
api_specs:
- filename: hiring-index-insights-api-openapi.yml
  format: yaml
  label: Hiring Index Insights API
  slug: hiring-index-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiring-index/refs/heads/main/openapi/hiring-index-insights-api-openapi.yml
- filename: hiring-index-job-api-openapi.yml
  format: yaml
  label: Hiring Index Job API
  slug: hiring-index-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiring-index/refs/heads/main/openapi/hiring-index-job-api-openapi.yml
- filename: hiring-index-search-api-openapi.yml
  format: yaml
  label: Hiring Index Search API
  slug: hiring-index-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiring-index/refs/heads/main/openapi/hiring-index-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hiringindex.org
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Dec 13 18:00:21 2026 GMT
  host: hiringindex.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: hiringindex.p.rapidapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Hiring Index Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hiring Index, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hiring Index
provider_slug: hiring-index
slug: hiring-index-domain-security
source_filename: hiring-index-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hiringindex.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 18:00:21 2026 GMT\n  hsts: false\n- host: hiringindex.p.rapidapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: hiringindex.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hiring-index/refs/heads/main/security/hiring-index-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Job
- Hiring Data
- Labor Market
- Human Resources
- Recruiting
- Job Postings
- Market Intelligence
- Alternative Data
---
