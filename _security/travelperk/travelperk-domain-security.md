---
api_specs:
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Bookings & Trips API
  slug: travelperk-bookings-trips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Invoices API
  slug: travelperk-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Expenses API
  slug: travelperk-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Travelers & Members API
  slug: travelperk-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Cost Centers API
  slug: travelperk-cost-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
- filename: travelperk-openapi.yml
  format: yaml
  label: TravelPerk Webhooks API
  slug: travelperk-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/openapi/travelperk-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: travelperk.com
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: www.travelperk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: developers.travelperk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: api.travelperk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Travelperk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TravelPerk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TravelPerk
provider_slug: travelperk
slug: travelperk-domain-security
source_filename: travelperk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.travelperk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: false\n- host: developers.travelperk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.travelperk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: travelperk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/travelperk/refs/heads/main/security/travelperk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Business Travel
- Travel Management
- Expenses
- Invoices
- Bookings
---
