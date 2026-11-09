---
api_specs:
- filename: airport-pickups-london-com-amend-booking-api-openapi.yml
  format: yaml
  label: Airport Pickups London Amend Booking API
  slug: airport-pickups-london-com-amend-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-amend-booking-api-openapi.yml
- filename: airport-pickups-london-com-book-api-openapi.yml
  format: yaml
  label: Airport Pickups London Book API
  slug: airport-pickups-london-com-book-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-book-api-openapi.yml
- filename: airport-pickups-london-com-cancel-booking-api-openapi.yml
  format: yaml
  label: Airport Pickups London Cancel Booking API
  slug: airport-pickups-london-com-cancel-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-cancel-booking-api-openapi.yml
- filename: airport-pickups-london-com-lookup-booking-api-openapi.yml
  format: yaml
  label: Airport Pickups London Lookup Booking API
  slug: airport-pickups-london-com-lookup-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-lookup-booking-api-openapi.yml
- filename: airport-pickups-london-com-quote-api-openapi.yml
  format: yaml
  label: Airport Pickups London Quote API
  slug: airport-pickups-london-com-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-quote-api-openapi.yml
- filename: airport-pickups-london-com-track-api-openapi.yml
  format: yaml
  label: Airport Pickups London Track API
  slug: airport-pickups-london-com-track-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-track-api-openapi.yml
- filename: airport-pickups-london-com-validate-flight-api-openapi.yml
  format: yaml
  label: Airport Pickups London Validate Flight API
  slug: airport-pickups-london-com-validate-flight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/airport-pickups-london-com/openapi/airport-pickups-london-com-validate-flight-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airport-pickups-london.com
  spf: true
hosts:
- cert_expires: Dec  7 02:21:33 2026 GMT
  host: airport-pickups-london.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Airport Pickups London Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airport Pickups London, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Airport Pickups London
provider_slug: airport-pickups-london-com
slug: airport-pickups-london-com-domain-security
source_filename: airport-pickups-london-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airport-pickups-london.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 02:21:33 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: airport-pickups-london.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/airport-pickups-london-com/security/airport-pickups-london-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Airport
- Transport
- Taxi
- London
---
