---
api_specs:
- filename: znanylekarz-addresses-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Addresses API
  slug: znanylekarz-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-addresses-api-openapi.yml
- filename: znanylekarz-api-notification-callbacks-api-openapi.yml
  format: yaml
  label: ZnanyLekarz API Notification Callbacks API
  slug: znanylekarz-api-notification-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-api-notification-callbacks-api-openapi.yml
- filename: znanylekarz-bookings-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Bookings API
  slug: znanylekarz-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-bookings-api-openapi.yml
- filename: znanylekarz-calendar-breaks-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Calendar Breaks API
  slug: znanylekarz-calendar-breaks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-calendar-breaks-api-openapi.yml
- filename: znanylekarz-calendars-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Calendars API
  slug: znanylekarz-calendars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-calendars-api-openapi.yml
- filename: znanylekarz-doctors-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Doctors API
  slug: znanylekarz-doctors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-doctors-api-openapi.yml
- filename: znanylekarz-facilities-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Facilities API
  slug: znanylekarz-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-facilities-api-openapi.yml
- filename: znanylekarz-insurances-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Insurances API
  slug: znanylekarz-insurances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-insurances-api-openapi.yml
- filename: znanylekarz-patient-presence-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Patient Presence API
  slug: znanylekarz-patient-presence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-patient-presence-api-openapi.yml
- filename: znanylekarz-services-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Services API
  slug: znanylekarz-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-services-api-openapi.yml
- filename: znanylekarz-slots-api-openapi.yml
  format: yaml
  label: ZnanyLekarz Slots API
  slug: znanylekarz-slots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/openapi/znanylekarz-slots-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: znanylekarz.pl
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: docplanner.com
  spf: true
hosts:
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: www.znanylekarz.pl
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: integrations.docplanner.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Znanylekarz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZnanyLekarz, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ZnanyLekarz
provider_slug: znanylekarz
slug: znanylekarz-domain-security
source_filename: znanylekarz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.znanylekarz.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: false\n- host: integrations.docplanner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: znanylekarz.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: docplanner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/znanylekarz/refs/heads/main/security/znanylekarz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Health Tech
- Appointments
- Booking
- Medical
- Marketplace
- Doctors
- Scheduling
- Poland
- Practice Management
- Telehealth
---
