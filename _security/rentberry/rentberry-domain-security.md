---
api_specs:
- filename: rentberry-openapi.yml
  format: yaml
  label: Rentberry API
  slug: rentberry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rentberry/refs/heads/main/openapi/rentberry-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rentberry.com
  spf: true
hosts:
- cert_expires: Oct 11 03:33:53 2026 GMT
  host: rentberry.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 03:33:53 2026 GMT
  host: api.rentberry.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: 'HSTS confirmed by a live GET on 2026-08-02 (the automated HEAD probe returned null). Observed header: strict-transport-security max-age=31536000; includeSubDomains; preload.'
  server: cloudflare
  tls_version: TLSv1.3
  x_content_type_options: nosniff
kind: domain-security
layout: security
method: probed
name: Rentberry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rentberry, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rentberry
provider_slug: rentberry
slug: rentberry-domain-security
source_filename: rentberry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rentberry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 03:33:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rentberry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 03:33:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  x_content_type_options: nosniff\n  server: cloudflare\n  note: >-\n    HSTS confirmed by a live GET on 2026-08-02 (the automated HEAD probe returned null).\n    Observed header: strict-transport-security max-age=31536000; includeSubDomains; preload.\ndomains:\n- domain: rentberry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentberry/refs/heads/main/security/rentberry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- real-estate
- proptech
- rentals
- rental-marketplace
- property-management
- tenant-screening
- e-signature
- payments
- listings
- search
- geocoding
- marketplace
---
