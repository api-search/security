---
api_specs:
- filename: apaleo-booking-api-openapi.yml
  format: yaml
  label: apaleo Booking API
  slug: apaleo-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-booking-api-openapi.yml
- filename: apaleo-authorization-api-openapi.yml
  format: yaml
  label: apaleo Authorization API
  slug: apaleo-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-authorization-api-openapi.yml
- filename: apaleo-authorizationactions-api-openapi.yml
  format: yaml
  label: apaleo Authorization Actions API
  slug: apaleo-authorizationactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-authorizationactions-api-openapi.yml
- filename: apaleo-block-api-openapi.yml
  format: yaml
  label: apaleo Block API
  slug: apaleo-block-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-block-api-openapi.yml
- filename: apaleo-blockactions-api-openapi.yml
  format: yaml
  label: apaleo Block Actions API
  slug: apaleo-blockactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-blockactions-api-openapi.yml
- filename: apaleo-group-api-openapi.yml
  format: yaml
  label: apaleo Group API
  slug: apaleo-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-group-api-openapi.yml
- filename: apaleo-groupactions-api-openapi.yml
  format: yaml
  label: apaleo Group Actions API
  slug: apaleo-groupactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-groupactions-api-openapi.yml
- filename: apaleo-offer-api-openapi.yml
  format: yaml
  label: apaleo Offer API
  slug: apaleo-offer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-offer-api-openapi.yml
- filename: apaleo-paymentaccountactions-api-openapi.yml
  format: yaml
  label: apaleo Payment Account Actions API
  slug: apaleo-paymentaccountactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-paymentaccountactions-api-openapi.yml
- filename: apaleo-reservation-api-openapi.yml
  format: yaml
  label: apaleo Reservation API
  slug: apaleo-reservation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-reservation-api-openapi.yml
- filename: apaleo-reservationactions-api-openapi.yml
  format: yaml
  label: apaleo Reservation Actions API
  slug: apaleo-reservationactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-reservationactions-api-openapi.yml
- filename: apaleo-types-api-openapi.yml
  format: yaml
  label: apaleo Types API
  slug: apaleo-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-types-api-openapi.yml
- filename: apaleo-payment-account-api-openapi.yml
  format: yaml
  label: apaleo Payment Account API
  slug: apaleo-payment-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apaleo/openapi/apaleo-payment-account-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apaleo.com
  spf: true
hosts:
- cert_expires: Sep  6 23:59:59 2026 GMT
  host: www.apaleo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  6 23:59:59 2026 GMT
  host: api.apaleo.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  6 23:59:59 2026 GMT
  host: webhook.apaleo.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: apaleo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for apaleo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: apaleo
provider_slug: apaleo
slug: apaleo-domain-security
source_filename: apaleo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apaleo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.apaleo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: webhook.apaleo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: apaleo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/apaleo/security/apaleo-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Hospitality
- PMS
- Property Management
- Hotels
- API-First
---
