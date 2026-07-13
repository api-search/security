---
api_specs:
- filename: deputy-openapi.yml
  format: yaml
  label: Deputy Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deputy/refs/heads/main/openapi/deputy-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:devops.admin@deputy.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "certainly.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deputy.com
  spf: true
hosts:
- cert_expires: Oct  9 16:52:48 2026 GMT
  host: www.deputy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 05:55:47 2026 GMT
  host: developer.deputy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deputy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deputy, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Deputy
provider_slug: deputy
slug: deputy-domain-security
source_filename: deputy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.deputy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:52:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.deputy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 05:55:47 2026 GMT\n  hsts: null\ndomains:\n- domain: deputy.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:devops.admin@deputy.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deputy/refs/heads/main/security/deputy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Workforce Management
- Employee Scheduling
- Time and Attendance
- Timesheets
- Human Resources
- Shift Planning
---
