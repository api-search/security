---
api_specs:
- filename: vuiapp-vn-openapi-generated.yml
  format: yaml
  label: Nano API
  slug: vuiapp-vn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vuiapp-vn/openapi/_ae-authored/vuiapp-vn-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vuiapp.vn
  spf: true
hosts:
- cert_expires: Dec  4 14:17:27 2026 GMT
  host: vuiapp.vn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vuiapp Vn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nano, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nano
provider_slug: vuiapp-vn
slug: vuiapp-vn-domain-security
source_filename: vuiapp-vn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vuiapp.vn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 14:17:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vuiapp.vn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/vuiapp-vn/security/vuiapp-vn-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
