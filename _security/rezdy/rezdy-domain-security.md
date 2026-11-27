---
api_specs:
- filename: rezdy-availability-api-openapi.yml
  format: yaml
  label: Rezdy Availability API
  slug: rezdy-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rezdy/openapi/rezdy-availability-api-openapi.yml
- filename: rezdy-bookings-api-openapi.yml
  format: yaml
  label: Rezdy Bookings API
  slug: rezdy-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rezdy/openapi/rezdy-bookings-api-openapi.yml
- filename: rezdy-categories-api-openapi.yml
  format: yaml
  label: Rezdy Categories API
  slug: rezdy-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rezdy/openapi/rezdy-categories-api-openapi.yml
- filename: rezdy-companies-api-openapi.yml
  format: yaml
  label: Rezdy Companies API
  slug: rezdy-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rezdy/openapi/rezdy-companies-api-openapi.yml
- filename: rezdy-manifest-api-openapi.yml
  format: yaml
  label: Rezdy Manifest API
  slug: rezdy-manifest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rezdy/openapi/rezdy-manifest-api-openapi.yml
- filename: rezdy-products-api-openapi.yml
  format: yaml
  label: Rezdy Products API
  slug: rezdy-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rezdy/openapi/rezdy-products-api-openapi.yml
- filename: rezdy-resources-api-openapi.yml
  format: yaml
  label: Rezdy Resources API
  slug: rezdy-resources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rezdy/openapi/rezdy-resources-api-openapi.yml
- filename: rezdy-vouchers-api-openapi.yml
  format: yaml
  label: Rezdy Vouchers API
  slug: rezdy-vouchers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rezdy/openapi/rezdy-vouchers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rezdy.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: rezdy-staging.com
  spf: false
hosts:
- cert_expires: Jan 13 16:51:01 2027 GMT
  host: rezdy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: developers.rezdy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: api.rezdy-staging.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Rezdy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rezdy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rezdy
provider_slug: rezdy
slug: rezdy-domain-security
source_filename: rezdy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rezdy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 16:51:01 2027 GMT\n  hsts: false\n- host: developers.rezdy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: false\n- host: api.rezdy-staging.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: rezdy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: rezdy-staging.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/rezdy/security/rezdy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Booking
- Software-as-a-Service
- Tourism
---
