---
api_specs:
- filename: openapi.json
  format: json
  label: SignSealShip Partner API
  slug: partner-api
  spec_type: OpenAPI
  url: https://docs.signsealship.com/api-reference/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: signsealship.com
  spf: true
hosts:
- cert_expires: Oct 11 14:19:16 2026 GMT
  host: docs.signsealship.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 04:14:24 2026 GMT
  host: signsealship.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Signsealship Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SignSealShip Partner API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SignSealShip Partner API
provider_slug: signsealship
slug: signsealship-domain-security
source_filename: signsealship-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.signsealship.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 14:19:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: signsealship.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 04:14:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: signsealship.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signsealship/refs/heads/main/security/signsealship-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- notarization
- remote online notarization
- electronic signature
- document verification
- legal technology
- real estate
- title and escrow
- shipping
---
