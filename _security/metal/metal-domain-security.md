---
api_specs:
- filename: metal-openapi-generated.yml
  format: yaml
  label: Metal API
  slug: metal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metal/refs/heads/main/openapi/_ae-authored/metal-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: metal.build
  spf: false
hosts:
- cert_expires: Nov 26 06:34:04 2026 GMT
  host: metal.build
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Metal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Metal
provider_slug: metal
slug: metal-domain-security
source_filename: metal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metal.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 06:34:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: metal.build\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metal/refs/heads/main/security/metal-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Platform
- Cloud
- DeveloperTools
- WebApplications
---
