---
api_specs:
- filename: university-of-toronto-courses-api-openapi.yml
  format: yaml
  label: University of Toronto Courses API
  slug: university-of-toronto-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-toronto/refs/heads/main/openapi/university-of-toronto-courses-api-openapi.yml
- filename: university-of-toronto-reference-data-api-openapi.yml
  format: yaml
  label: University of Toronto Reference Data API
  slug: university-of-toronto-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-toronto/refs/heads/main/openapi/university-of-toronto-reference-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: utoronto.ca
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scholaris.ca
  spf: true
hosts:
- cert_expires: Sep 22 03:50:38 2026 GMT
  host: www.utoronto.ca
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  5 23:59:59 2027 GMT
  host: utoronto.scholaris.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Toronto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Toronto, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Toronto
provider_slug: university-of-toronto
slug: university-of-toronto-domain-security
source_filename: university-of-toronto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.utoronto.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 03:50:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: utoronto.scholaris.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: utoronto.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: scholaris.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-toronto/refs/heads/main/security/university-of-toronto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- Canada
- U15
- Research
- Course Catalog
- Identity Federation
- Research Data
- Institutional Repository
- Library
- Public Research University
---
