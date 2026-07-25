---
api_specs:
- filename: microsoft-bookings-appointments-api-openapi.yml
  format: yaml
  label: Microsoft Bookings Appointments API
  slug: microsoft-bookings-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/openapi/microsoft-bookings-appointments-api-openapi.yml
- filename: microsoft-bookings-bookingbusinesses-api-openapi.yml
  format: yaml
  label: Microsoft Bookings BookingBusinesses API
  slug: microsoft-bookings-bookingbusinesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/openapi/microsoft-bookings-bookingbusinesses-api-openapi.yml
- filename: microsoft-bookings-currencies-api-openapi.yml
  format: yaml
  label: Microsoft Bookings Currencies API
  slug: microsoft-bookings-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/openapi/microsoft-bookings-currencies-api-openapi.yml
- filename: microsoft-bookings-customers-api-openapi.yml
  format: yaml
  label: Microsoft Bookings Customers API
  slug: microsoft-bookings-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/openapi/microsoft-bookings-customers-api-openapi.yml
- filename: microsoft-bookings-customquestions-api-openapi.yml
  format: yaml
  label: Microsoft Bookings CustomQuestions API
  slug: microsoft-bookings-customquestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/openapi/microsoft-bookings-customquestions-api-openapi.yml
- filename: microsoft-bookings-services-api-openapi.yml
  format: yaml
  label: Microsoft Bookings Services API
  slug: microsoft-bookings-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/openapi/microsoft-bookings-services-api-openapi.yml
- filename: microsoft-bookings-staffmembers-api-openapi.yml
  format: yaml
  label: Microsoft Bookings StaffMembers API
  slug: microsoft-bookings-staffmembers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/openapi/microsoft-bookings-staffmembers-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 03:53:00 2026 GMT
  host: graph.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Bookings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Bookings, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Bookings
provider_slug: microsoft-bookings
slug: microsoft-bookings-domain-security
source_filename: microsoft-bookings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: graph.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 03:53:00 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-bookings/refs/heads/main/security/microsoft-bookings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bookings
- Scheduling
- Appointments
- Microsoft Graph
---
