---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Przelewy24 REST API
  slug: przelewy24-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi.yml
- filename: openapi-marketplace.yml
  format: yaml
  label: Przelewy24 Marketplace API
  slug: przelewy24-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/openapi-marketplace.yml
- filename: openapi-extended.yml
  format: yaml
  label: Przelewy24 Extended API
  slug: przelewy24-extended-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/openapi-extended.yml
- filename: openapi-ekspres.yml
  format: yaml
  label: Przelewy24 Ekspres API
  slug: przelewy24-ekspres-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/openapi/openapi-ekspres.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: przelewy24.pl
  spf: true
hosts:
- cert_expires: Jul 31 23:59:59 2026 GMT
  host: www.przelewy24.pl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 31 23:59:59 2026 GMT
  host: developers.przelewy24.pl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: secure.przelewy24.pl
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Przelewy24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Przelewy24, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Przelewy24
provider_slug: przelewy24
slug: przelewy24-domain-security
source_filename: przelewy24-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.przelewy24.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.przelewy24.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: secure.przelewy24.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: przelewy24.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/przelewy24/refs/heads/main/security/przelewy24-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Gateway
- Bank Transfer
- BLIK
- Card Payments
- E-Commerce
- Poland
- Polish
- Multi-Currency
- Fintech
---
