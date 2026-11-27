---
api_specs:
- filename: dfetcher-com-openapi-generated.yml
  format: yaml
  label: D Fetcher API
  slug: dfetcher-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dfetcher-com/openapi/_ae-authored/dfetcher-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dfetcher.com
  spf: true
hosts:
- cert_expires: Dec 22 06:43:51 2026 GMT
  host: dfetcher.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: D Fetcher Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for D Fetcher, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: D Fetcher
provider_slug: dfetcher-com
slug: dfetcher-com-domain-security
source_filename: dfetcher-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dfetcher.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 06:43:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dfetcher.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dfetcher-com/security/dfetcher-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Vitamin D
- Health
- Calculator
- OpenAPI
- Free
---
