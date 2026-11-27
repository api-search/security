---
api_specs:
- filename: ktemia-openapi-generated.yml
  format: yaml
  label: Ktemia API
  slug: ktemia-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ktemia/openapi/_ae-authored/ktemia-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ktemia.com
  spf: true
hosts:
- cert_expires: Apr  5 11:31:36 2027 GMT
  host: www.ktemia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ktemia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ktemia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ktemia
provider_slug: ktemia
slug: ktemia-domain-security
source_filename: ktemia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ktemia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 11:31:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ktemia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ktemia/security/ktemia-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Travel
- Search
- Flights
- Hotels
- Cars
- Real Estate
---
