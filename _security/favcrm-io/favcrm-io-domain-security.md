---
api_specs:
- filename: favcrm-io-content-api-openapi.yml
  format: yaml
  label: FavCRM Content API
  slug: favcrm-io-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/favcrm-io/openapi/favcrm-io-content-api-openapi.yml
- filename: favcrm-io-events-api-openapi.yml
  format: yaml
  label: FavCRM Events API
  slug: favcrm-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/favcrm-io/openapi/favcrm-io-events-api-openapi.yml
- filename: favcrm-io-forms-and-surveys-api-openapi.yml
  format: yaml
  label: FavCRM Forms and Surveys API
  slug: favcrm-io-forms-and-surveys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/favcrm-io/openapi/favcrm-io-forms-and-surveys-api-openapi.yml
- filename: favcrm-io-loyalty-and-offers-api-openapi.yml
  format: yaml
  label: FavCRM Loyalty and Offers API
  slug: favcrm-io-loyalty-and-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/favcrm-io/openapi/favcrm-io-loyalty-and-offers-api-openapi.yml
- filename: favcrm-io-member-session-api-openapi.yml
  format: yaml
  label: FavCRM Member Session API
  slug: favcrm-io-member-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/favcrm-io/openapi/favcrm-io-member-session-api-openapi.yml
- filename: favcrm-io-service-booking-api-openapi.yml
  format: yaml
  label: FavCRM Service Booking API
  slug: favcrm-io-service-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/favcrm-io/openapi/favcrm-io-service-booking-api-openapi.yml
- filename: favcrm-io-shop-api-openapi.yml
  format: yaml
  label: FavCRM Shop API
  slug: favcrm-io-shop-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/favcrm-io/openapi/favcrm-io-shop-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: favcrm.io
  spf: true
hosts:
- cert_expires: Dec 12 11:40:27 2026 GMT
  host: favcrm.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Favcrm Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FavCRM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FavCRM
provider_slug: favcrm-io
slug: favcrm-io-domain-security
source_filename: favcrm-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: favcrm.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 11:40:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: favcrm.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/favcrm-io/security/favcrm-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CRM
- Appointment
- Membership
- WhatsApp
- AI
---
