---
api_specs:
- filename: bindbee-candidates-api-openapi.yml
  format: yaml
  label: Bindbee Candidates API
  slug: bindbee-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-candidates-api-openapi.yml
- filename: bindbee-departments-api-openapi.yml
  format: yaml
  label: Bindbee Departments API
  slug: bindbee-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-departments-api-openapi.yml
- filename: bindbee-employees-api-openapi.yml
  format: yaml
  label: Bindbee Employees API
  slug: bindbee-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-employees-api-openapi.yml
- filename: bindbee-jobs-api-openapi.yml
  format: yaml
  label: Bindbee Jobs API
  slug: bindbee-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-jobs-api-openapi.yml
- filename: bindbee-time-off-api-openapi.yml
  format: yaml
  label: Bindbee Time Off API
  slug: bindbee-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-time-off-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bindbee.dev
  spf: true
hosts:
- cert_expires: Sep  5 08:42:16 2026 GMT
  host: bindbee.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 05:43:57 2026 GMT
  host: api.bindbee.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bindbee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bindbee, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bindbee
provider_slug: bindbee
slug: bindbee-domain-security
source_filename: bindbee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bindbee.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 08:42:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bindbee.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 05:43:57 2026 GMT\n  hsts: null\ndomains:\n- domain: bindbee.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/security/bindbee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ATS
- HR Integration
- HRIS
- Workforce
---
