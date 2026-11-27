---
api_specs:
- filename: footage-cool-openapi-generated.yml
  format: yaml
  label: footage.cool API
  slug: footage-cool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/footage-cool/openapi/_ae-authored/footage-cool-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: footage.cool
  spf: true
hosts:
- cert_expires: Dec 23 03:03:55 2026 GMT
  host: footage.cool
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: footage.cool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for footage.cool, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: footage.cool
provider_slug: footage-cool
slug: footage-cool-domain-security
source_filename: footage-cool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: footage.cool\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 03:03:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: footage.cool\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/footage-cool/security/footage-cool-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- StockFootage
- Cinematic
- DirectLicensing
- PhilMaher
- Media
---
