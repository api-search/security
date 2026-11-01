---
api_specs:
- filename: openapi.json
  format: json
  label: Grundfast API
  slug: grundfast-api
  spec_type: OpenAPI
  url: https://grundfast.dk/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: grundfast.dk
  spf: true
hosts:
- cert_expires: Jan 15 10:37:10 2027 GMT
  host: grundfast.dk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Grundfast Dk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for grundfast-dk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: grundfast-dk
provider_slug: grundfast-dk
slug: grundfast-dk-domain-security
source_filename: grundfast-dk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grundfast.dk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 10:37:10 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: grundfast.dk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/grundfast-dk/security/grundfast-dk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- RealEstate
- Geodata
- API
- Denmark
- Compatibility
---
