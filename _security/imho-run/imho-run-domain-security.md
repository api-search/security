---
api_specs:
- filename: imho-run-openapi-generated.yml
  format: yaml
  label: imho.run API
  slug: imho-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imho-run/openapi/_ae-authored/imho-run-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: imho.run
  spf: true
hosts:
- cert_expires: Jan 30 08:54:34 2027 GMT
  host: imho.run
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: imho.run Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for imho.run, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: imho.run
provider_slug: imho-run
slug: imho-run-domain-security
source_filename: imho-run-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imho.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 08:54:34 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: imho.run\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/imho-run/security/imho-run-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Gaming
- Recommendations
- Steam
- Free
---
