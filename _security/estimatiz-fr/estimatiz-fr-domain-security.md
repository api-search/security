---
api_specs:
- filename: estimatiz-fr-public-api-openapi.yml
  format: yaml
  label: Estimatiz Public API
  slug: estimatiz-fr-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/estimatiz-fr/openapi/estimatiz-fr-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: estimatiz.fr
  spf: true
hosts:
- cert_expires: Jan 27 15:37:05 2027 GMT
  host: estimatiz.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Estimatiz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Estimatiz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Estimatiz
provider_slug: estimatiz-fr
slug: estimatiz-fr-domain-security
source_filename: estimatiz-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: estimatiz.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 15:37:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: estimatiz.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/estimatiz-fr/security/estimatiz-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Valuation
- France
- Open Data
---
