---
api_specs:
- filename: ucla-class-sections-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Class Sections API
  slug: ucla-class-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-class-sections-api-openapi.yml
- filename: ucla-classes-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Classes API
  slug: ucla-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-classes-api-openapi.yml
- filename: ucla-courses-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Courses API
  slug: ucla-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-courses-api-openapi.yml
- filename: ucla-dictionary-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Dictionary API
  slug: ucla-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-dictionary-api-openapi.yml
- filename: ucla-ge-foundations-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles GE Foundations API
  slug: ucla-ge-foundations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-ge-foundations-api-openapi.yml
- filename: ucla-infrastructure-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Infrastructure API
  slug: ucla-infrastructure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-infrastructure-api-openapi.yml
- filename: ucla-myucla-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles My UCLA API
  slug: ucla-myucla-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-myucla-api-openapi.yml
- filename: ucla-production-calendar-jobs-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Production Calendar Jobs API
  slug: ucla-production-calendar-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-production-calendar-jobs-api-openapi.yml
- filename: ucla-weather-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Weather API
  slug: ucla-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-weather-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ucla.edu
  spf: true
hosts:
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: www.ucla.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 14:52:29 2026 GMT
  host: developer.api.ucla.edu
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
- cert_expires: Apr  9 23:59:59 2027 GMT
  host: api.ucla.edu
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ucla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of California, Los Angeles, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of California, Los Angeles
provider_slug: ucla
slug: ucla-domain-security
source_filename: ucla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ucla.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\n- host: developer.api.ucla.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 14:52:29 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: api.ucla.edu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ucla.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/security/ucla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- United States
- California
- UC System
- Public Research University
- Course Catalog
- Student Information
- Identity Federation
- Research Repository
- Library
- IIIF
- Campus Life
---
