---
api_specs:
- filename: ratehawk-openapi.yml
  format: yaml
  label: RateHawk Hotel Search API
  slug: hotel-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-openapi.yml
- filename: ratehawk-openapi.yml
  format: yaml
  label: RateHawk Hotel Page / Prebook API
  slug: hotel-page-prebook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-openapi.yml
- filename: ratehawk-openapi.yml
  format: yaml
  label: RateHawk Order Booking API
  slug: order-booking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-openapi.yml
- filename: ratehawk-openapi.yml
  format: yaml
  label: RateHawk Hotel Content / Static API
  slug: hotel-content-static
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-openapi.yml
- filename: ratehawk-openapi.yml
  format: yaml
  label: RateHawk Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/openapi/ratehawk-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ratehawk.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: emergingtravel.com
  spf: true
hosts:
- cert_expires: Oct  6 15:32:51 2026 GMT
  host: www.ratehawk.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 11:27:15 2026 GMT
  host: docs.emergingtravel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 09:17:17 2027 GMT
  host: api.worldota.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ratehawk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RateHawk, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RateHawk
provider_slug: ratehawk
slug: ratehawk-domain-security
source_filename: ratehawk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ratehawk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 15:32:51 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.emergingtravel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:27:15 2026 GMT\n  hsts: false\n- host: api.worldota.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 09:17:17 2027 GMT\n  hsts: false\ndomains:\n- domain: ratehawk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: emergingtravel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ratehawk/refs/heads/main/security/ratehawk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Hotels
- Booking
- B2B
- Reservations
---
