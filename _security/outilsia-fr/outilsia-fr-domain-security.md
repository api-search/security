---
api_specs:
- filename: outilsia-fr-favicon-ico-api-openapi.yml
  format: yaml
  label: OutilsIA Favicon.ico API
  slug: outilsia-fr-favicon-ico-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outilsia-fr/openapi/outilsia-fr-favicon-ico-api-openapi.yml
- filename: outilsia-fr-health-api-openapi.yml
  format: yaml
  label: OutilsIA Health API
  slug: outilsia-fr-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outilsia-fr/openapi/outilsia-fr-health-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: outilsia.fr
  spf: false
hosts:
- cert_expires: Dec 25 13:38:29 2026 GMT
  host: outilsia.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OutilsIA Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OutilsIA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OutilsIA
provider_slug: outilsia-fr
slug: outilsia-fr-domain-security
source_filename: outilsia-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outilsia.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 13:38:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: outilsia.fr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/outilsia-fr/security/outilsia-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Rust
- Local-IA
- French
- Software
---
