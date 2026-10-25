---
api_specs:
- filename: ch-robinson-worldwide-authentication-api-openapi.yml
  format: yaml
  label: C.H. Robinson Authentication API
  slug: ch-robinson-worldwide-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/openapi/ch-robinson-worldwide-authentication-api-openapi.yml
- filename: ch-robinson-worldwide-documents-api-openapi.yml
  format: yaml
  label: C.H. Robinson Documents API
  slug: ch-robinson-worldwide-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/openapi/ch-robinson-worldwide-documents-api-openapi.yml
- filename: ch-robinson-worldwide-events-api-openapi.yml
  format: yaml
  label: C.H. Robinson Events API
  slug: ch-robinson-worldwide-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/openapi/ch-robinson-worldwide-events-api-openapi.yml
- filename: ch-robinson-worldwide-financials-api-openapi.yml
  format: yaml
  label: C.H. Robinson Financials API
  slug: ch-robinson-worldwide-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/openapi/ch-robinson-worldwide-financials-api-openapi.yml
- filename: ch-robinson-worldwide-labels-api-openapi.yml
  format: yaml
  label: C.H. Robinson Labels API
  slug: ch-robinson-worldwide-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/openapi/ch-robinson-worldwide-labels-api-openapi.yml
- filename: ch-robinson-worldwide-orders-and-booking-api-openapi.yml
  format: yaml
  label: C.H. Robinson Orders and Booking API
  slug: ch-robinson-worldwide-orders-and-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/openapi/ch-robinson-worldwide-orders-and-booking-api-openapi.yml
- filename: ch-robinson-worldwide-rating-api-openapi.yml
  format: yaml
  label: C.H. Robinson Rating API
  slug: ch-robinson-worldwide-rating-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/openapi/ch-robinson-worldwide-rating-api-openapi.yml
- filename: ch-robinson-worldwide-shipments-api-openapi.yml
  format: yaml
  label: C.H. Robinson Shipments API
  slug: ch-robinson-worldwide-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/openapi/ch-robinson-worldwide-shipments-api-openapi.yml
- filename: ch-robinson-worldwide-visibility-api-openapi.yml
  format: yaml
  label: C.H. Robinson Visibility API
  slug: ch-robinson-worldwide-visibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/openapi/ch-robinson-worldwide-visibility-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: chrobinson.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: navisphere.com
  spf: true
hosts:
- cert_expires: Dec  5 04:38:06 2026 GMT
  host: www.chrobinson.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 04:05:14 2026 GMT
  host: developer.chrobinson.com
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 11 06:00:08 2027 GMT
  host: api.navisphere.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Ch Robinson Worldwide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for C.H. Robinson, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: C.H. Robinson
provider_slug: ch-robinson-worldwide
slug: ch-robinson-worldwide-domain-security
source_filename: ch-robinson-worldwide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.chrobinson.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 04:38:06 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: developer.chrobinson.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 04:05:14 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\n- host: api.navisphere.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 06:00:08 2027 GMT\n  hsts: null\ndomains:\n- domain: chrobinson.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: navisphere.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ch-robinson-worldwide/refs/heads/main/security/ch-robinson-worldwide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Freight
- Logistics
- Shipping
- Supply Chain
- Transportation
- Transportation Management
- Fortune 500
---
