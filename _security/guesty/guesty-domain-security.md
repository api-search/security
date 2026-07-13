---
api_specs:
- filename: guesty-openapi.yml
  format: yaml
  label: Guesty Open API
  slug: guesty-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guesty/refs/heads/main/openapi/guesty-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: guesty.com
  spf: true
hosts:
- cert_expires: Sep  7 22:59:50 2026 GMT
  host: open-api-docs.guesty.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: www.guesty.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 17 23:59:59 2027 GMT
  host: open-api.guesty.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Guesty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guesty, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Guesty
provider_slug: guesty
slug: guesty-domain-security
source_filename: guesty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open-api-docs.guesty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 22:59:50 2026 GMT\n  hsts: null\n- host: www.guesty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: open-api.guesty.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 17 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: guesty.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guesty/refs/heads/main/security/guesty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Booking
- Hospitality
- Property Management
- Reservations
- Short-Term Rentals
- Vacation Rentals
---
