---
api_specs:
- filename: nogogo-fr-openapi-generated.yml
  format: yaml
  label: Nogogo API
  slug: nogogo-fr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nogogo-fr/openapi/_ae-authored/nogogo-fr-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nogogo.fr
  spf: true
hosts:
- cert_expires: Jan 28 14:40:03 2027 GMT
  host: nogogo.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nogogo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nogogo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nogogo
provider_slug: nogogo-fr
slug: nogogo-fr-domain-security
source_filename: nogogo-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nogogo.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 14:40:03 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nogogo.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nogogo-fr/security/nogogo-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- French
- Data
- Risk Management
- Analytics
- Platform
---
