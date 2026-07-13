---
api_specs:
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Partner API
  slug: eat-app-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Concierge Reservations API
  slug: eat-app-concierge-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Concierge Guests API
  slug: eat-app-concierge-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Concierge Availability API
  slug: eat-app-concierge-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Concierge Restaurants and Groups API
  slug: eat-app-concierge-restaurants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
- filename: eat-app-openapi.yml
  format: yaml
  label: Eat App Tables and Floorplan API
  slug: eat-app-tables-floorplan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/openapi/eat-app-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: eatapp.co
  spf: true
hosts:
- cert_expires: Aug 22 13:54:56 2026 GMT
  host: eatapp.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 20:25:28 2026 GMT
  host: restaurant.eatapp.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 13:54:56 2026 GMT
  host: api.eatapp.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eat App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eat App, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Eat App
provider_slug: eat-app
slug: eat-app-domain-security
source_filename: eat-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eatapp.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 13:54:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: restaurant.eatapp.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 20:25:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.eatapp.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 13:54:56 2026 GMT\n  hsts: null\ndomains:\n- domain: eatapp.co\n  dnssec: true\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eat-app/refs/heads/main/security/eat-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Restaurant
- Reservations
- Table Management
- Hospitality
- Bookings
- Guest CRM
- Availability
---
