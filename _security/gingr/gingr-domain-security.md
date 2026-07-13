---
api_specs:
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Owners API
  slug: gingr-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Pets API
  slug: gingr-pets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Reservations API
  slug: gingr-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Services API
  slug: gingr-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Invoices & Payments API
  slug: gingr-invoices-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Vaccinations API
  slug: gingr-vaccinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Report Cards API
  slug: gingr-report-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
- filename: gingr-openapi.yml
  format: yaml
  label: Gingr Waitlist API
  slug: gingr-waitlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/openapi/gingr-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gingrapp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gingr.io
  spf: true
hosts:
- cert_expires: Sep 15 17:06:19 2026 GMT
  host: www.gingrapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:43:39 2026 GMT
  host: support.gingrapp.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: api.gingr.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gingr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gingr, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gingr
provider_slug: gingr
slug: gingr-domain-security
source_filename: gingr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gingrapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 17:06:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.gingrapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:43:39 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.gingr.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: gingrapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: gingr.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gingr/refs/heads/main/security/gingr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pet Care
- Pet Daycare
- Boarding
- Grooming
- Vertical SaaS
- Scheduling
- Payments
---
