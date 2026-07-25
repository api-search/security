---
api_specs:
- filename: google-calendar-calendars-api-openapi.yml
  format: yaml
  label: Google Calendar Calendars API
  slug: google-calendar-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-calendar/refs/heads/main/openapi/google-calendar-calendars-api-openapi.yml
- filename: google-calendar-colors-api-openapi.yml
  format: yaml
  label: Google Calendar Colors API
  slug: google-calendar-colors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-calendar/refs/heads/main/openapi/google-calendar-colors-api-openapi.yml
- filename: google-calendar-freebusy-api-openapi.yml
  format: yaml
  label: Google Calendar freeBusy API
  slug: google-calendar-freebusy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-calendar/refs/heads/main/openapi/google-calendar-freebusy-api-openapi.yml
- filename: google-calendar-users-api-openapi.yml
  format: yaml
  label: Google Calendar Users API
  slug: google-calendar-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-calendar/refs/heads/main/openapi/google-calendar-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: www.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Calendar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Calendar, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Calendar
provider_slug: google-calendar
slug: google-calendar-domain-security
source_filename: google-calendar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-calendar/refs/heads/main/security/google-calendar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Availability
- Calendar
- Events
- Google
- Google Workspace
- Scheduling
---
