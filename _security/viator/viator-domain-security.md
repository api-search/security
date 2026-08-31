---
api_specs:
- filename: viator-attraction-services-api-openapi.yml
  format: yaml
  label: Viator Attraction services API
  slug: viator-attraction-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-attraction-services-api-openapi.yml
- filename: viator-attractions-api-openapi.yml
  format: yaml
  label: Viator Attractions API
  slug: viator-attractions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-attractions-api-openapi.yml
- filename: viator-auxiliary-api-openapi.yml
  format: yaml
  label: Viator Auxiliary API
  slug: viator-auxiliary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-auxiliary-api-openapi.yml
- filename: viator-availability-api-openapi.yml
  format: yaml
  label: Viator Availability API
  slug: viator-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-availability-api-openapi.yml
- filename: viator-booking-services-api-openapi.yml
  format: yaml
  label: Viator Booking services API
  slug: viator-booking-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-booking-services-api-openapi.yml
- filename: viator-bookings-api-openapi.yml
  format: yaml
  label: Viator Bookings API
  slug: viator-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-bookings-api-openapi.yml
- filename: viator-deprecated-api-openapi.yml
  format: yaml
  label: Viator Deprecated API
  slug: viator-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-deprecated-api-openapi.yml
- filename: viator-deprecated-services-api-openapi.yml
  format: yaml
  label: Viator Deprecated services API
  slug: viator-deprecated-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-deprecated-services-api-openapi.yml
- filename: viator-general-services-api-openapi.yml
  format: yaml
  label: Viator General services API
  slug: viator-general-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-general-services-api-openapi.yml
- filename: viator-payments-api-openapi.yml
  format: yaml
  label: Viator Payments API
  slug: viator-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-payments-api-openapi.yml
- filename: viator-product-services-api-openapi.yml
  format: yaml
  label: Viator Product services API
  slug: viator-product-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-product-services-api-openapi.yml
- filename: viator-products-api-openapi.yml
  format: yaml
  label: Viator Products API
  slug: viator-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-products-api-openapi.yml
- filename: viator-reservation-system-apis-api-openapi.yml
  format: yaml
  label: Viator Reservation system APIs API
  slug: viator-reservation-system-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-reservation-system-apis-api-openapi.yml
- filename: viator-support-services-api-openapi.yml
  format: yaml
  label: Viator Support services API
  slug: viator-support-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-support-services-api-openapi.yml
- filename: viator-taxonomy-services-api-openapi.yml
  format: yaml
  label: Viator Taxonomy services API
  slug: viator-taxonomy-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-taxonomy-services-api-openapi.yml
- filename: viator-utility-services-api-openapi.yml
  format: yaml
  label: Viator Utility services API
  slug: viator-utility-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-utility-services-api-openapi.yml
- filename: viator-viator-apis-api-openapi.yml
  format: yaml
  label: Viator Viator APIs API
  slug: viator-viator-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viator/refs/heads/main/openapi/viator-viator-apis-api-openapi.yml
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
