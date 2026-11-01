---
api_specs:
- filename: addevent-calendar-subscribers-api-openapi.yml
  format: yaml
  label: AddEvent Calendar subscribers API
  slug: addevent-calendar-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-calendar-subscribers-api-openapi.yml
- filename: addevent-calendars-api-openapi.yml
  format: yaml
  label: AddEvent Calendars API
  slug: addevent-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-calendars-api-openapi.yml
- filename: addevent-events-api-openapi.yml
  format: yaml
  label: AddEvent Events API
  slug: addevent-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-events-api-openapi.yml
- filename: addevent-rsvp-attendees-api-openapi.yml
  format: yaml
  label: AddEvent RSVP attendees API
  slug: addevent-rsvp-attendees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-rsvp-attendees-api-openapi.yml
- filename: addevent-templates-api-openapi.yml
  format: yaml
  label: AddEvent Templates API
  slug: addevent-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-templates-api-openapi.yml
- filename: addevent-timezones-api-openapi.yml
  format: yaml
  label: AddEvent Timezones API
  slug: addevent-timezones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/addevent/openapi/addevent-timezones-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: addevent.com
  spf: true
hosts:
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: addevent.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Addevent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AddEvent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AddEvent
provider_slug: addevent
slug: addevent-domain-security
source_filename: addevent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: addevent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: addevent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/addevent/security/addevent-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Calendar
- Integration
- Marketing
- API
- SaaS
- Events
---
