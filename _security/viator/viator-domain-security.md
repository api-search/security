---
api_specs:
- filename: viator-partner-api-v2-openapi.json
  format: json
  label: Viator Partner Products API
  slug: viator-partner-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-partner-api-v2-openapi.json
- filename: viator-partner-api-v2-openapi.json
  format: json
  label: Viator Partner Availability API
  slug: viator-partner-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-partner-api-v2-openapi.json
- filename: viator-partner-api-v2-openapi.json
  format: json
  label: Viator Partner Bookings API
  slug: viator-partner-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-partner-api-v2-openapi.json
- filename: viator-partner-api-v2-openapi.json
  format: json
  label: Viator Partner Payments API
  slug: viator-partner-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-partner-api-v2-openapi.json
- filename: viator-partner-api-v2-openapi.json
  format: json
  label: Viator Partner Attractions API
  slug: viator-partner-attractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-partner-api-v2-openapi.json
- filename: viator-partner-api-v2-openapi.json
  format: json
  label: Viator Partner Auxiliary API
  slug: viator-partner-auxiliary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-partner-api-v2-openapi.json
- filename: viator-reservation-system-api-openapi.json
  format: json
  label: Viator Reservation System API
  slug: viator-reservation-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-reservation-system-api-openapi.json
- filename: viator-merchant-api-v1-openapi.json
  format: json
  label: Viator Merchant API v1
  slug: viator-merchant-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-merchant-api-v1-openapi.json
- filename: viator-affiliate-api-v1-openapi.json
  format: json
  label: Viator Affiliate API v1
  slug: viator-affiliate-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-affiliate-api-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: viator.com
  spf: true
hosts:
- cert_expires: Aug 24 18:23:02 2026 GMT
  host: www.viator.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:39:31 2026 GMT
  host: partnerresources.viator.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 06:33:46 2026 GMT
  host: docs.viator.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: api.viator.com
  hsts: false
  https: true
  note: Partner API v2 production host; answers 400 without exp-api-key + Accept version header.
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: api.sandbox.viator.com
  hsts: false
  https: true
  note: Partner API v2 sandbox host declared in the OpenAPI servers[] block.
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: viatorapi.viator.com
  hsts: false
  https: true
  note: Legacy v1 affiliate/merchant host; returned 503 to unauthenticated probes.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Viator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Viator, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Viator
provider_slug: viator
slug: viator-domain-security
source_filename: viator-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.viator.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:23:02 2026 GMT\n  hsts: null\n- host: partnerresources.viator.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:39:31 2026 GMT\n  hsts: false\n- host: docs.viator.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 06:33:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.viator.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\n  note: Partner API v2 production host; answers 400 without exp-api-key + Accept version header.\n- host: api.sandbox.viator.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: false\n  note: Partner API v2 sandbox host declared in the OpenAPI servers[] block.\n- host: viatorapi.viator.com\n  https: true\n  tls_version:\
  \ TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: false\n  note: Legacy v1 affiliate/merchant host; returned 503 to unauthenticated probes.\ndomains:\n- domain: viator.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/security/viator-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- United States
- Tours and Activities
- Experience
- OTA
- Booking
- Distribution
- Marketplace
- Affiliates
- Hospitality
---
