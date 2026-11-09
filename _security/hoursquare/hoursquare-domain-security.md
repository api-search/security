---
api_specs:
- filename: hoursquare-attendance-api-openapi.yml
  format: yaml
  label: HourSquare Attendance API
  slug: hoursquare-attendance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-attendance-api-openapi.yml
- filename: hoursquare-employees-api-openapi.yml
  format: yaml
  label: HourSquare Employees API
  slug: hoursquare-employees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-employees-api-openapi.yml
- filename: hoursquare-me-api-openapi.yml
  format: yaml
  label: HourSquare Me API
  slug: hoursquare-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-me-api-openapi.yml
- filename: hoursquare-oauth-api-openapi.yml
  format: yaml
  label: HourSquare OAuth API
  slug: hoursquare-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoursquare/openapi/hoursquare-oauth-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hoursquare.com
  spf: true
hosts:
- cert_expires: Jan 24 03:14:59 2027 GMT
  host: hoursquare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hoursquare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HourSquare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HourSquare
provider_slug: hoursquare
slug: hoursquare-domain-security
source_filename: hoursquare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hoursquare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 03:14:59 2027 GMT\n  hsts: false\ndomains:\n- domain: hoursquare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/hoursquare/security/hoursquare-domain-security.yml
summary_line: TLSv1.3
tags:
- Human Resources
- Payroll
- Time Tracking
- Workforce Management
- Software-as-a-Service
---
