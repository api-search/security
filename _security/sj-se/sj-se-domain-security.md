---
api_specs:
- filename: sj-se-availabilities-api-openapi.yml
  format: yaml
  label: SJ Availabilities API
  slug: sj-se-availabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sj-se/refs/heads/main/openapi/sj-se-availabilities-api-openapi.yml
- filename: sj-se-booking-api-openapi.yml
  format: yaml
  label: SJ Booking API
  slug: sj-se-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sj-se/refs/heads/main/openapi/sj-se-booking-api-openapi.yml
- filename: sj-se-bookings-api-openapi.yml
  format: yaml
  label: SJ Bookings API
  slug: sj-se-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sj-se/refs/heads/main/openapi/sj-se-bookings-api-openapi.yml
- filename: sj-se-contacts-api-openapi.yml
  format: yaml
  label: SJ Contacts API
  slug: sj-se-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sj-se/refs/heads/main/openapi/sj-se-contacts-api-openapi.yml
- filename: sj-se-exchange-offers-api-openapi.yml
  format: yaml
  label: SJ Exchange Offers API
  slug: sj-se-exchange-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sj-se/refs/heads/main/openapi/sj-se-exchange-offers-api-openapi.yml
- filename: sj-se-exchange-operations-api-openapi.yml
  format: yaml
  label: SJ Exchange Operations API
  slug: sj-se-exchange-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sj-se/refs/heads/main/openapi/sj-se-exchange-operations-api-openapi.yml
- filename: sj-se-fulfillments-api-openapi.yml
  format: yaml
  label: SJ Fulfillments API
  slug: sj-se-fulfillments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sj-se/refs/heads/main/openapi/sj-se-fulfillments-api-openapi.yml
- filename: sj-se-offers-api-openapi.yml
  format: yaml
  label: SJ Offers API
  slug: sj-se-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sj-se/refs/heads/main/openapi/sj-se-offers-api-openapi.yml
- filename: sj-se-passenger-api-openapi.yml
  format: yaml
  label: SJ Passenger API
  slug: sj-se-passenger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sj-se/refs/heads/main/openapi/sj-se-passenger-api-openapi.yml
- filename: sj-se-tenant-id-api-openapi.yml
  format: yaml
  label: SJ Tenant Id API
  slug: sj-se-tenant-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sj-se/refs/heads/main/openapi/sj-se-tenant-id-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sj.se
  spf: true
hosts:
- cert_expires: Dec  3 03:26:13 2026 GMT
  host: sj.se
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sj Se Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SJ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SJ
provider_slug: sj-se
slug: sj-se-domain-security
source_filename: sj-se-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sj.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 03:26:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: sj.se\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sj-se/refs/heads/main/security/sj-se-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
---
