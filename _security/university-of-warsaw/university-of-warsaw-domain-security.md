---
api_specs:
- filename: university-of-warsaw-apiref-api-openapi.yml
  format: yaml
  label: University of Warsaw apiref API
  slug: university-of-warsaw-apiref-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/openapi/university-of-warsaw-apiref-api-openapi.yml
- filename: university-of-warsaw-apisrv-api-openapi.yml
  format: yaml
  label: University of Warsaw apisrv API
  slug: university-of-warsaw-apisrv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/openapi/university-of-warsaw-apisrv-api-openapi.yml
- filename: university-of-warsaw-calendar-api-openapi.yml
  format: yaml
  label: University of Warsaw calendar API
  slug: university-of-warsaw-calendar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/openapi/university-of-warsaw-calendar-api-openapi.yml
- filename: university-of-warsaw-courses-api-openapi.yml
  format: yaml
  label: University of Warsaw courses API
  slug: university-of-warsaw-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/openapi/university-of-warsaw-courses-api-openapi.yml
- filename: university-of-warsaw-fac-api-openapi.yml
  format: yaml
  label: University of Warsaw fac API
  slug: university-of-warsaw-fac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/openapi/university-of-warsaw-fac-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uw.edu.pl
  spf: true
hosts:
- cert_expires: Jan 10 09:56:50 2027 GMT
  host: en.uw.edu.pl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  3 12:03:20 2026 GMT
  host: usosapps.uw.edu.pl
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 24 05:48:23 2026 GMT
  host: danebadawcze.uw.edu.pl
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Warsaw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Warsaw, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Warsaw
provider_slug: university-of-warsaw
slug: university-of-warsaw-domain-security
source_filename: university-of-warsaw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.uw.edu.pl\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 10 09:56:50 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: usosapps.uw.edu.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 12:03:20 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: danebadawcze.uw.edu.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 05:48:23 2026 GMT\n  hsts: false\ndomains:\n- domain: uw.edu.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/security/university-of-warsaw-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Poland
- Academic Data
- Research Data
- Open Data
---
