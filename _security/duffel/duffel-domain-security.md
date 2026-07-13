---
api_specs:
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Offer Requests API
  slug: duffel-offer-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Offers API
  slug: duffel-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Orders API
  slug: duffel-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Seat Maps API
  slug: duffel-seat-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Order Changes API
  slug: duffel-order-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Order Cancellations API
  slug: duffel-order-cancellations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Payments API
  slug: duffel-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Stays API
  slug: duffel-stays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
- filename: duffel-openapi.yml
  format: yaml
  label: Duffel Webhooks API
  slug: duffel-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/openapi/duffel-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@duffel.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: duffel.com
  spf: true
hosts:
- cert_expires: Aug 29 11:00:00 2026 GMT
  host: duffel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 13:32:30 2026 GMT
  host: api.duffel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Duffel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Duffel, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Duffel
provider_slug: duffel
slug: duffel-domain-security
source_filename: duffel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: duffel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 11:00:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.duffel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 13:32:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: duffel.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@duffel.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duffel/refs/heads/main/security/duffel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Travel
- Flights
- Hotels
- Booking
- Payments
---
