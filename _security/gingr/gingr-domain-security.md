---
api_specs:
- filename: gingr-invoices-api-openapi.yml
  format: yaml
  label: Gingr Invoices API
  slug: gingr-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-invoices-api-openapi.yml
- filename: gingr-payments-api-openapi.yml
  format: yaml
  label: Gingr Payments API
  slug: gingr-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-payments-api-openapi.yml
- filename: gingr-pets-api-openapi.yml
  format: yaml
  label: Gingr Pets API
  slug: gingr-pets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-pets-api-openapi.yml
- filename: gingr-booking-type-rates-api-openapi.yml
  format: yaml
  label: Gingr Booking Type Rates API
  slug: gingr-booking-type-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-booking-type-rates-api-openapi.yml
- filename: gingr-bookings-api-openapi.yml
  format: yaml
  label: Gingr Bookings API
  slug: gingr-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-bookings-api-openapi.yml
- filename: gingr-card-on-file-api-openapi.yml
  format: yaml
  label: Gingr Card On File API
  slug: gingr-card-on-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-card-on-file-api-openapi.yml
- filename: gingr-config-api-openapi.yml
  format: yaml
  label: Gingr Config API
  slug: gingr-config-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-config-api-openapi.yml
- filename: gingr-group-classes-api-openapi.yml
  format: yaml
  label: Gingr Group Classes API
  slug: gingr-group-classes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-group-classes-api-openapi.yml
- filename: gingr-parents-api-openapi.yml
  format: yaml
  label: Gingr Parents API
  slug: gingr-parents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-parents-api-openapi.yml
- filename: gingr-payment-api-openapi.yml
  format: yaml
  label: Gingr Payment API
  slug: gingr-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-payment-api-openapi.yml
- filename: gingr-precheck-api-openapi.yml
  format: yaml
  label: Gingr Precheck API
  slug: gingr-precheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-precheck-api-openapi.yml
- filename: gingr-upload-api-openapi.yml
  format: yaml
  label: Gingr Upload API
  slug: gingr-upload-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gingr/openapi/gingr-upload-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gingrapp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gingr.io
  spf: true
hosts:
- cert_expires: Sep 15 17:06:19 2026 GMT
  host: www.gingrapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:43:39 2026 GMT
  host: support.gingrapp.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: api.gingr.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Gingr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gingr, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gingr
provider_slug: gingr
slug: gingr-domain-security
source_filename: gingr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gingrapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 17:06:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.gingrapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:43:39 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.gingr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: gingrapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: gingr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gingr/security/gingr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pet Care
- Pet Daycare
- Boarding
- Grooming
- Vertical SaaS
- Scheduling
- Payments
---
