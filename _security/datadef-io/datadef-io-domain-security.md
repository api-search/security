---
api_specs:
- filename: datadef-io-openapi-generated.yml
  format: yaml
  label: Datadef API
  slug: datadef-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datadef-io/openapi/_ae-authored/datadef-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: datadef.io
  spf: true
hosts:
- cert_expires: Jan 17 14:18:52 2027 GMT
  host: datadef.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datadef Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datadef, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Datadef
provider_slug: datadef-io
slug: datadef-io-domain-security
source_filename: datadef-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datadef.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 14:18:52 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: datadef.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/datadef-io/security/datadef-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Data Engineering
- AI Tools
- Diagramming
- Cloud Architecture
- Open Source
---
