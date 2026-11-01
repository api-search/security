---
api_specs:
- filename: firmtape-com-levels-api-openapi.yml
  format: yaml
  label: firmtape-com Levels API
  slug: firmtape-com-levels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmtape-com/openapi/firmtape-com-levels-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: firmtape.com
  spf: true
hosts:
- cert_expires: Jan 27 22:26:51 2027 GMT
  host: firmtape.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Firmtape Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for firmtape-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: firmtape-com
provider_slug: firmtape-com
slug: firmtape-com-domain-security
source_filename: firmtape-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firmtape.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 22:26:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: firmtape.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/firmtape-com/security/firmtape-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Data
- Analytics
- Options
- Gamma
---
