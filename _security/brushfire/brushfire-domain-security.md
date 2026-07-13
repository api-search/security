---
api_specs:
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Events API
  slug: brushfire-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Attendees API
  slug: brushfire-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Orders API
  slug: brushfire-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Cart & Checkout API
  slug: brushfire-cart-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Sessions & Check-In API
  slug: brushfire-sessions-checkin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Groups API
  slug: brushfire-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Promotions & Access Codes API
  slug: brushfire-promotions-accesscodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
- filename: brushfire-openapi.json
  format: json
  label: Brushfire Webhooks (Hooks) API
  slug: brushfire-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:technology@brushfire.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brushfire.com
  spf: true
hosts:
- cert_expires: Sep 29 17:54:52 2026 GMT
  host: www.brushfire.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 13:41:23 2026 GMT
  host: developer.brushfire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 13:41:23 2026 GMT
  host: api.brushfire.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brushfire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brushfire, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brushfire
provider_slug: brushfire
slug: brushfire-domain-security
source_filename: brushfire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brushfire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:54:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.brushfire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 13:41:23 2026 GMT\n  hsts: false\n- host: api.brushfire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 13:41:23 2026 GMT\n  hsts: null\ndomains:\n- domain: brushfire.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:technology@brushfire.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/security/brushfire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Event Ticketing
- Registration
- Events
- Ticketing
- Check-In
- Churches
- Payments
---
