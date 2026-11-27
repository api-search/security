---
api_specs:
- filename: datosia-net-openapi-generated.yml
  format: yaml
  label: DatosIA API
  slug: datosia-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datosia-net/openapi/_ae-authored/datosia-net-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: datosia.net
  spf: true
hosts:
- cert_expires: Jan  5 15:55:11 2027 GMT
  host: datosia.net
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DatosIA Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DatosIA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DatosIA
provider_slug: datosia-net
slug: datosia-net-domain-security
source_filename: datosia-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datosia.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 15:55:11 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: datosia.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/datosia-net/security/datosia-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Central America
- Open Data
- Statistics
---
