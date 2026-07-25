---
api_specs:
- filename: quandoo-availabilities-api-openapi.yml
  format: yaml
  label: Quandoo Availabilities API
  slug: quandoo-availabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-availabilities-api-openapi.yml
- filename: quandoo-customers-api-openapi.yml
  format: yaml
  label: Quandoo Customers API
  slug: quandoo-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-customers-api-openapi.yml
- filename: quandoo-merchants-api-openapi.yml
  format: yaml
  label: Quandoo Merchants API
  slug: quandoo-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-merchants-api-openapi.yml
- filename: quandoo-reservation-enquiries-api-openapi.yml
  format: yaml
  label: Quandoo Reservation Enquiries API
  slug: quandoo-reservation-enquiries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-reservation-enquiries-api-openapi.yml
- filename: quandoo-reservation-settings-api-openapi.yml
  format: yaml
  label: Quandoo Reservation Settings API
  slug: quandoo-reservation-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-reservation-settings-api-openapi.yml
- filename: quandoo-reservations-api-openapi.yml
  format: yaml
  label: Quandoo Reservations API
  slug: quandoo-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-reservations-api-openapi.yml
- filename: quandoo-reservations-tags-api-openapi.yml
  format: yaml
  label: Quandoo Reservations Tags API
  slug: quandoo-reservations-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-reservations-tags-api-openapi.yml
- filename: quandoo-reviews-api-openapi.yml
  format: yaml
  label: Quandoo Reviews API
  slug: quandoo-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-reviews-api-openapi.yml
- filename: quandoo-status-api-openapi.yml
  format: yaml
  label: Quandoo Status API
  slug: quandoo-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-status-api-openapi.yml
- filename: quandoo-validations-api-openapi.yml
  format: yaml
  label: Quandoo Validations API
  slug: quandoo-validations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/openapi/quandoo-validations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quandoo.com
  spf: true
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: www.quandoo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: docs.quandoo.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: public-api.prod.quandoo.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Quandoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quandoo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quandoo
provider_slug: quandoo
slug: quandoo-domain-security
source_filename: quandoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quandoo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.quandoo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: false\n- host: public-api.prod.quandoo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: quandoo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quandoo/refs/heads/main/security/quandoo-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Restaurant
- Reservations
- Booking
- Availability
- Merchants
- Marketplace
---
