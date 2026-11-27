---
api_specs:
- filename: microsoft-bookings-solutions-bookingbusiness-api-openapi.yml
  format: yaml
  label: Microsoft Bookings Solutions.booking Business API
  slug: microsoft-bookings-solutions-bookingbusiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bookings/openapi/microsoft-bookings-solutions-bookingbusiness-api-openapi.yml
- filename: microsoft-bookings-solutions-bookingcurrency-api-openapi.yml
  format: yaml
  label: Microsoft Bookings Solutions.booking Currency API
  slug: microsoft-bookings-solutions-bookingcurrency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-bookings/openapi/microsoft-bookings-solutions-bookingcurrency-api-openapi.yml
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
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 15:26:39 2027 GMT
  host: graph.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Microsoft Bookings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Bookings, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Bookings
provider_slug: microsoft-bookings
slug: microsoft-bookings-domain-security
source_filename: microsoft-bookings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: graph.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 15:26:39 2027 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-bookings/security/microsoft-bookings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Booking
- Scheduling
- Appointments
- Microsoft Graph
- Calendar
- Microsoft 365
---
