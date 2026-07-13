---
api_specs:
- filename: metronome-openapi.json
  format: json
  label: Metronome API
  slug: metronome-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/openapi/metronome-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: metronome.com
  spf: true
hosts:
- cert_expires: Nov  2 23:59:59 2026 GMT
  host: metronome.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 16:04:32 2026 GMT
  host: docs.metronome.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: api.metronome.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metronome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metronome, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Metronome
provider_slug: metronome
slug: metronome-domain-security
source_filename: metronome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metronome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.metronome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 16:04:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.metronome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: metronome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metronome/refs/heads/main/security/metronome-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Billing
- FinOps
- Metering
- Pricing
- Usage-Based Billing
---
