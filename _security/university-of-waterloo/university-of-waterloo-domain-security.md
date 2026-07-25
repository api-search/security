---
api_specs:
- filename: university-of-waterloo-academicorganizations-api-openapi.yml
  format: yaml
  label: University of Waterloo AcademicOrganizations API
  slug: university-of-waterloo-academicorganizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-academicorganizations-api-openapi.yml
- filename: university-of-waterloo-account-api-openapi.yml
  format: yaml
  label: University of Waterloo Account API
  slug: university-of-waterloo-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-account-api-openapi.yml
- filename: university-of-waterloo-classschedules-api-openapi.yml
  format: yaml
  label: University of Waterloo ClassSchedules API
  slug: university-of-waterloo-classschedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-classschedules-api-openapi.yml
- filename: university-of-waterloo-courses-api-openapi.yml
  format: yaml
  label: University of Waterloo Courses API
  slug: university-of-waterloo-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-courses-api-openapi.yml
- filename: university-of-waterloo-examschedules-api-openapi.yml
  format: yaml
  label: University of Waterloo ExamSchedules API
  slug: university-of-waterloo-examschedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-examschedules-api-openapi.yml
- filename: university-of-waterloo-foodservices-api-openapi.yml
  format: yaml
  label: University of Waterloo FoodServices API
  slug: university-of-waterloo-foodservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-foodservices-api-openapi.yml
- filename: university-of-waterloo-holidaydates-api-openapi.yml
  format: yaml
  label: University of Waterloo HolidayDates API
  slug: university-of-waterloo-holidaydates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-holidaydates-api-openapi.yml
- filename: university-of-waterloo-importantdates-api-openapi.yml
  format: yaml
  label: University of Waterloo ImportantDates API
  slug: university-of-waterloo-importantdates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-importantdates-api-openapi.yml
- filename: university-of-waterloo-locations-api-openapi.yml
  format: yaml
  label: University of Waterloo Locations API
  slug: university-of-waterloo-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-locations-api-openapi.yml
- filename: university-of-waterloo-subjects-api-openapi.yml
  format: yaml
  label: University of Waterloo Subjects API
  slug: university-of-waterloo-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-subjects-api-openapi.yml
- filename: university-of-waterloo-terms-api-openapi.yml
  format: yaml
  label: University of Waterloo Terms API
  slug: university-of-waterloo-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-terms-api-openapi.yml
- filename: university-of-waterloo-wcms-api-openapi.yml
  format: yaml
  label: University of Waterloo Wcms API
  slug: university-of-waterloo-wcms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-wcms-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uwaterloo.ca
  spf: true
hosts:
- cert_expires: Aug  3 00:36:52 2026 GMT
  host: uwaterloo.ca
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: openapi.data.uwaterloo.ca
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Waterloo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Waterloo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Waterloo
provider_slug: university-of-waterloo
slug: university-of-waterloo-domain-security
source_filename: university-of-waterloo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uwaterloo.ca\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  3 00:36:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: openapi.data.uwaterloo.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: uwaterloo.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/security/university-of-waterloo-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Canada
- Research
---
