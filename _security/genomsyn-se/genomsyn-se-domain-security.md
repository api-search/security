---
api_specs:
- filename: genomsyn-se-foretag-api-openapi.yml
  format: yaml
  label: Bolagsdata Foretag API
  slug: genomsyn-se-foretag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genomsyn-se/openapi/genomsyn-se-foretag-api-openapi.yml
- filename: genomsyn-se-sok-api-openapi.yml
  format: yaml
  label: Bolagsdata Sok API
  slug: genomsyn-se-sok-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genomsyn-se/openapi/genomsyn-se-sok-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: genomsyn.se
  spf: false
hosts:
- cert_expires: Feb  5 08:10:16 2027 GMT
  host: genomsyn.se
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bolagsdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bolagsdata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Bolagsdata
provider_slug: genomsyn-se
slug: genomsyn-se-domain-security
source_filename: genomsyn-se-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genomsyn.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 08:10:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: genomsyn.se\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/genomsyn-se/security/genomsyn-se-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Finance
- Swedish
- Companies
- Data
- Open
---
