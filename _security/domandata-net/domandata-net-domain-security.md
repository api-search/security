---
api_specs:
- filename: domandata-net-openapi-generated.yml
  format: yaml
  label: Domandata API
  slug: domandata-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domandata-net/openapi/_ae-authored/domandata-net-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: domandata.net
  spf: true
hosts:
- cert_expires: Jan 12 13:46:00 2027 GMT
  host: domandata.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Domandata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Domandata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Domandata
provider_slug: domandata-net
slug: domandata-net-domain-security
source_filename: domandata-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: domandata.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 13:46:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: domandata.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/domandata-net/security/domandata-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Surveys
- Academic
- Research
- Software
---
