---
api_specs:
- filename: openapi.json
  format: json
  label: Luma API
  slug: luma-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: luma.com
  spf: true
hosts:
- cert_expires: Sep  7 02:00:29 2026 GMT
  host: docs.luma.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 17:43:45 2026 GMT
  host: public-api.luma.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Luma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luma, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Luma
provider_slug: luma
slug: luma-domain-security
source_filename: luma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.luma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 02:00:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public-api.luma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 17:43:45 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: luma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luma/refs/heads/main/security/luma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Events
- Event Management
- Ticketing
- Community
- Calendars
- Guests
- Attendance
---
