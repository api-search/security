---
api_specs:
- filename: outdoorsy-openapi-original.json
  format: json
  label: Outdoorsy API
  slug: outdoorsy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outdoorsy/refs/heads/main/openapi/outdoorsy-openapi-original.json
- filename: outdoorsy-search-openapi-original.json
  format: json
  label: Outdoorsy Search API
  slug: outdoorsy-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outdoorsy/refs/heads/main/openapi/outdoorsy-search-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: outdoorsy.com
  spf: true
hosts:
- cert_expires: Sep 30 10:51:33 2026 GMT
  host: www.outdoorsy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 10:51:33 2026 GMT
  host: developers.outdoorsy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 10:51:33 2026 GMT
  host: api.outdoorsy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outdoorsy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outdoorsy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Outdoorsy
provider_slug: outdoorsy
slug: outdoorsy-domain-security
source_filename: outdoorsy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.outdoorsy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:51:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.outdoorsy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:51:33 2026 GMT\n  hsts: false\n- host: api.outdoorsy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:51:33 2026 GMT\n  hsts: null\ndomains:\n- domain: outdoorsy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outdoorsy/refs/heads/main/security/outdoorsy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Marketplace
- Rentals
- Recreational Vehicles
- Bookings
- Search
- Payments
- Insurance
- Camping
- Tourism
---
