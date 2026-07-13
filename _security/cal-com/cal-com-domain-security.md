---
api_specs:
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Bookings API
  slug: cal-com-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Event Types API
  slug: cal-com-event-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Schedules API
  slug: cal-com-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Availability API
  slug: cal-com-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Slots API
  slug: cal-com-slots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Webhooks API
  slug: cal-com-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com OAuth & Auth API
  slug: cal-com-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Teams API
  slug: cal-com-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Organizations API
  slug: cal-com-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Out-of-Office API
  slug: cal-com-ooo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Conferencing API
  slug: cal-com-conferencing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Destination Calendars API
  slug: cal-com-destination-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
- filename: cal-com-openapi.json
  format: json
  label: Cal.com Atoms (Platform)
  slug: cal-com-atoms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/openapi/cal-com-openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issue "www.digicert.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cal.com
  spf: true
hosts:
- cert_expires: Sep 14 15:26:52 2026 GMT
  host: cal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 12:46:41 2026 GMT
  host: api.cal.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cal Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cal.com, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cal.com
provider_slug: cal-com
slug: cal-com-domain-security
source_filename: cal-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:26:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 12:46:41 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cal.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"www.digicert.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cal-com/refs/heads/main/security/cal-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Productivity
- Scheduling
- Calendar
- Open Source
- Booking
---
