---
api_specs:
- filename: when-i-work-openapi.yml
  format: yaml
  label: When I Work API
  slug: when-i-work-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/when-i-work/refs/heads/main/openapi/when-i-work-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wheniwork.com
  spf: true
hosts:
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: wheniwork.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: apidocs.wheniwork.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: api.wheniwork.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: When I Work Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for When I Work, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: When I Work
provider_slug: when-i-work
slug: when-i-work-domain-security
source_filename: when-i-work-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wheniwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: false\n- host: apidocs.wheniwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: false\n- host: api.wheniwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wheniwork.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/when-i-work/refs/heads/main/security/when-i-work-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Employee Scheduling
- Workforce Management
- Time Tracking
- Time Clock
- Shift Management
- Attendance
- Team Messaging
- Hourly Workers
- Labor Forecasting
- HR
---
