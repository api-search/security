---
api_specs:
- filename: united-rentals-total-control-openapi.yml
  format: yaml
  label: United Rentals Total Control Integration API
  slug: united-rentals-total-control-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-rentals/main/openapi/united-rentals-total-control-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unitedrentals.com
  spf: true
hosts:
- cert_expires: Aug 13 23:59:59 2026 GMT
  host: www.unitedrentals.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- host: api.unitedrentals.com
  https: false
kind: domain-security
layout: security
method: probed
name: United Rentals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for United Rentals, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: United Rentals
provider_slug: united-rentals
slug: united-rentals-domain-security
source_filename: united-rentals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unitedrentals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: api.unitedrentals.com\n  https: false\ndomains:\n- domain: unitedrentals.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-rentals/refs/heads/main/security/united-rentals-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Equipment Rental
- Procurement
- Supply Chain
- Construction
- Fortune 500
---
