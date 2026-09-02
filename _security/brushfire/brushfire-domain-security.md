---
api_specs:
- filename: brushfire-accesscodes-api-openapi.yml
  format: yaml
  label: Brushfire AccessCodes API
  slug: brushfire-accesscodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-accesscodes-api-openapi.yml
- filename: brushfire-accounts-api-openapi.yml
  format: yaml
  label: Brushfire Accounts API
  slug: brushfire-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-accounts-api-openapi.yml
- filename: brushfire-attendees-api-openapi.yml
  format: yaml
  label: Brushfire Attendees API
  slug: brushfire-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-attendees-api-openapi.yml
- filename: brushfire-cart-api-openapi.yml
  format: yaml
  label: Brushfire Cart API
  slug: brushfire-cart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-cart-api-openapi.yml
- filename: brushfire-clients-api-openapi.yml
  format: yaml
  label: Brushfire Clients API
  slug: brushfire-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-clients-api-openapi.yml
- filename: brushfire-data-api-openapi.yml
  format: yaml
  label: Brushfire Data API
  slug: brushfire-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-data-api-openapi.yml
- filename: brushfire-events-api-openapi.yml
  format: yaml
  label: Brushfire Events API
  slug: brushfire-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-events-api-openapi.yml
- filename: brushfire-exchanges-api-openapi.yml
  format: yaml
  label: Brushfire Exchanges API
  slug: brushfire-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-exchanges-api-openapi.yml
- filename: brushfire-groups-api-openapi.yml
  format: yaml
  label: Brushfire Groups API
  slug: brushfire-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-groups-api-openapi.yml
- filename: brushfire-hooks-api-openapi.yml
  format: yaml
  label: Brushfire Hooks API
  slug: brushfire-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-hooks-api-openapi.yml
- filename: brushfire-lookups-api-openapi.yml
  format: yaml
  label: Brushfire Lookups API
  slug: brushfire-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-lookups-api-openapi.yml
- filename: brushfire-orders-api-openapi.yml
  format: yaml
  label: Brushfire Orders API
  slug: brushfire-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-orders-api-openapi.yml
- filename: brushfire-paymentprofiles-api-openapi.yml
  format: yaml
  label: Brushfire PaymentProfiles API
  slug: brushfire-paymentprofiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-paymentprofiles-api-openapi.yml
- filename: brushfire-promotions-api-openapi.yml
  format: yaml
  label: Brushfire Promotions API
  slug: brushfire-promotions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-promotions-api-openapi.yml
- filename: brushfire-regions-api-openapi.yml
  format: yaml
  label: Brushfire Regions API
  slug: brushfire-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-regions-api-openapi.yml
- filename: brushfire-sessions-api-openapi.yml
  format: yaml
  label: Brushfire Sessions API
  slug: brushfire-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brushfire/refs/heads/main/openapi/brushfire-sessions-api-openapi.yml
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
- Event
- Ticketing
- Check-in
- Churches
- Payments
---
