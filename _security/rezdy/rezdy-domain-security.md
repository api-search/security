---
api_specs:
- filename: rezdy-availability-api-openapi.yml
  format: yaml
  label: Rezdy Availability API
  slug: rezdy-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rezdy/refs/heads/main/openapi/rezdy-availability-api-openapi.yml
- filename: rezdy-bookings-api-openapi.yml
  format: yaml
  label: Rezdy Bookings API
  slug: rezdy-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rezdy/refs/heads/main/openapi/rezdy-bookings-api-openapi.yml
- filename: rezdy-categories-api-openapi.yml
  format: yaml
  label: Rezdy Categories API
  slug: rezdy-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rezdy/refs/heads/main/openapi/rezdy-categories-api-openapi.yml
- filename: rezdy-companies-api-openapi.yml
  format: yaml
  label: Rezdy Companies API
  slug: rezdy-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rezdy/refs/heads/main/openapi/rezdy-companies-api-openapi.yml
- filename: rezdy-manifest-api-openapi.yml
  format: yaml
  label: Rezdy Manifest API
  slug: rezdy-manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rezdy/refs/heads/main/openapi/rezdy-manifest-api-openapi.yml
- filename: rezdy-products-api-openapi.yml
  format: yaml
  label: Rezdy Products API
  slug: rezdy-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rezdy/refs/heads/main/openapi/rezdy-products-api-openapi.yml
- filename: rezdy-resources-api-openapi.yml
  format: yaml
  label: Rezdy Resources API
  slug: rezdy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rezdy/refs/heads/main/openapi/rezdy-resources-api-openapi.yml
- filename: rezdy-vouchers-api-openapi.yml
  format: yaml
  label: Rezdy Vouchers API
  slug: rezdy-vouchers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rezdy/refs/heads/main/openapi/rezdy-vouchers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rezdy.com
  spf: true
hosts:
- cert_expires: Dec 26 23:43:33 2026 GMT
  host: rezdy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rezdy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rezdy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rezdy
provider_slug: rezdy
slug: rezdy-domain-security
source_filename: rezdy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rezdy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 23:43:33 2026 GMT\n  hsts: false\ndomains:\n- domain: rezdy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rezdy/refs/heads/main/security/rezdy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Booking
- Software-as-a-Service
---
