---
api_specs:
- filename: hoplix-com-v1-openapi.json
  format: json
  label: Hoplix Print-on-Demand API
  slug: hoplix-print-on-demand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hoplix-com/openapi/_original/hoplix-com-v1-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hoplix.com
  spf: true
hosts:
- cert_expires: Feb  2 00:47:10 2027 GMT
  host: hoplix.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 20:59:50 2027 GMT
  host: api.hoplix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Hoplix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hoplix, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hoplix
provider_slug: hoplix-com
slug: hoplix-com-domain-security
source_filename: hoplix-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hoplix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 00:47:10 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.hoplix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 20:59:50 2027 GMT\n  hsts: false\ndomains:\n- domain: hoplix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hoplix-com/security/hoplix-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Print on Demand
- Dropshipping
- E-Commerce
- Merchandise
---
