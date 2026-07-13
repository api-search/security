---
api_specs:
- filename: calendarific-openapi.yml
  format: yaml
  label: Calendarific Holiday API
  slug: calendarific-holiday-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendarific/refs/heads/main/openapi/calendarific-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: calendarific.com
  spf: true
hosts:
- cert_expires: Sep 13 12:24:23 2026 GMT
  host: calendarific.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Calendarific Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calendarific, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Calendarific
provider_slug: calendarific
slug: calendarific-domain-security
source_filename: calendarific-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: calendarific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 12:24:23 2026 GMT\n  hsts: false\ndomains:\n- domain: calendarific.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calendarific/refs/heads/main/security/calendarific-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Calendar
- Public APIs
- Holidays
- Worldwide
- Localization
---
