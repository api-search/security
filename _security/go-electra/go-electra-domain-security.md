---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: go-electra.com
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: www.go-electra.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:50:05 2026 GMT
  host: ocpi.go-electra.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_note: 'The probe recorded null because the host root (/) returns 404 with no HSTS header. A follow-up HEAD of the real API route https://ocpi.go-electra.com/ocpi/cpo/versions on 2026-08-17 returned 200 with `strict-transport-security: max-age=63072000; includeSubDomains`, so HSTS is present with a two-year max-age on the API surface itself.'
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Go Electra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Electra, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Electra
provider_slug: go-electra
slug: go-electra-domain-security
source_filename: go-electra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.go-electra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: false\n- host: ocpi.go-electra.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:50:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    The probe recorded null because the host root (/) returns 404 with no HSTS\n    header. A follow-up HEAD of the real API route\n    https://ocpi.go-electra.com/ocpi/cpo/versions on 2026-08-17 returned 200\n    with `strict-transport-security: max-age=63072000; includeSubDomains`, so\n    HSTS is present with a two-year max-age on the API surface itself.\nnotes:\n- >-\n  www.go-electra.com is a CloudFront + S3 static site (server: CloudFront on the\n  301, AmazonS3 on the 200) and serves no HSTS header, so the marketing host is\n  the weaker of\
  \ the two. The API host ocpi.go-electra.com is behind Cloudflare\n  in front of a Rails application and does send HSTS.\n- >-\n  ocpi.go-electra.com also returns a restrictive Content-Security-Policy\n  (default-src 'self') on JSON API responses, and the standard Rails hardening\n  set (X-Frame-Options SAMEORIGIN, X-Content-Type-Options nosniff,\n  Referrer-Policy strict-origin-when-cross-origin,\n  X-Permitted-Cross-Domain-Policies none).\n- >-\n  The observed CSP connect-src on ocpi.go-electra.com includes\n  http://localhost:3004 and http://localhost:3035 — development origins left in\n  a production policy header. Recorded as observed; it is a hygiene note, not a\n  vulnerability finding.\ndomains:\n- domain: go-electra.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/go-electra/refs/heads/main/security/go-electra-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Climate Tech
- EV Charging
- Energy
- Mobility
- OCPI
- Roaming
- Charge Point Operator
- Electric Vehicles
- Fast Charging
- Charging Sessions
- Tariffs
- Electrification
- France
- Europe
---
