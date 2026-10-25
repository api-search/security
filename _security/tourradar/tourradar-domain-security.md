---
api_specs:
- filename: tourradar-bookings-api-openapi.yml
  format: yaml
  label: TourRadar Bookings API
  slug: tourradar-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/openapi/tourradar-bookings-api-openapi.yml
- filename: tourradar-bulk-api-openapi.yml
  format: yaml
  label: TourRadar Bulk API
  slug: tourradar-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/openapi/tourradar-bulk-api-openapi.yml
- filename: tourradar-operators-api-openapi.yml
  format: yaml
  label: TourRadar Operators API
  slug: tourradar-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/openapi/tourradar-operators-api-openapi.yml
- filename: tourradar-pricing-availability-api-openapi.yml
  format: yaml
  label: TourRadar Pricing & Availability API
  slug: tourradar-pricing-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/openapi/tourradar-pricing-availability-api-openapi.yml
- filename: tourradar-taxonomy-api-openapi.yml
  format: yaml
  label: TourRadar Taxonomy API
  slug: tourradar-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/openapi/tourradar-taxonomy-api-openapi.yml
- filename: tourradar-tours-api-openapi.yml
  format: yaml
  label: TourRadar Tours API
  slug: tourradar-tours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/openapi/tourradar-tours-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:security@tourradar.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tourradar.com
  spf: true
hosts:
- cert_expires: Mar 24 23:59:59 2027 GMT
  host: www.tourradar.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 31 23:59:59 2027 GMT
  host: api.b2b.tourradar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Tourradar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TourRadar, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TourRadar
provider_slug: tourradar
slug: tourradar-domain-security
source_filename: tourradar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tourradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.b2b.tourradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 31 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: tourradar.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:security@tourradar.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tourradar/refs/heads/main/security/tourradar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Tours
- Booking
- Marketplace
- Adventure Travel
- Distribution
- Affiliates
---
