---
api_specs:
- filename: calendly-scheduling-api-openapi.yml
  format: yaml
  label: Calendly Scheduling API
  slug: scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/openapi/calendly-scheduling-api-openapi.yml
- filename: calendly-webhook-api-asyncapi.yml
  format: yaml
  label: Calendly Webhook API
  slug: webhook-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/asyncapi/calendly-webhook-api-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:platform@calendly.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: calendly.com
  spf: true
hosts:
- cert_expires: Oct  5 14:35:08 2026 GMT
  host: developer.calendly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 14:35:08 2026 GMT
  host: calendly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 14:35:08 2026 GMT
  host: api.calendly.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Calendly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Calendly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Calendly
provider_slug: calendly
slug: calendly-domain-security
source_filename: calendly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.calendly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:35:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: calendly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:35:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.calendly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:35:08 2026 GMT\n  hsts: null\ndomains:\n- domain: calendly.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:platform@calendly.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/calendly/refs/heads/main/security/calendly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Appointments
- Automation
- Booking
- Calendars
- Meetings
- Scheduling
---
