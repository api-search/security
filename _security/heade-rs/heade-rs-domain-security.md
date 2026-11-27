---
api_specs:
- filename: heade-rs-heade-rs-api-api-openapi.yml
  format: yaml
  label: Heade.rs Heade.rs API
  slug: heade-rs-heade-rs-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heade-rs/openapi/heade-rs-heade-rs-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: heade.rs
  spf: true
hosts:
- cert_expires: Dec 24 19:57:13 2026 GMT
  host: heade.rs
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Heade.rs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heade.rs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Heade.rs
provider_slug: heade-rs
slug: heade-rs-domain-security
source_filename: heade-rs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heade.rs\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 19:57:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: heade.rs\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/heade-rs/security/heade-rs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- DNS
- IP
- Networks
- Tool
---
