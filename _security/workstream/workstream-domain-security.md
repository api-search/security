---
api_specs:
- filename: workstream-public-api-openapi-original.json
  format: json
  label: Workstream Public API
  slug: workstream-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/openapi/workstream-public-api-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workstream.us
  spf: true
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: workstream.us
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 19:06:01 2026 GMT
  host: docs.workstream.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: public-api.workstream.us
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workstream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workstream, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workstream
provider_slug: workstream
slug: workstream-domain-security
source_filename: workstream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: workstream.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\n- host: docs.workstream.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 19:06:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public-api.workstream.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: workstream.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workstream/refs/heads/main/security/workstream-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hr Tech
- Hiring
- Payroll
- Onboarding
- Applicant Tracking
- Hourly Workforce
- Restaurants
---
