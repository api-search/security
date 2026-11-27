---
api_specs:
- filename: melvea-com-free-api-openapi.yml
  format: yaml
  label: Melvea Free API
  slug: melvea-com-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/melvea-com/openapi/melvea-com-free-api-openapi.yml
- filename: melvea-com-x402-api-openapi.yml
  format: yaml
  label: Melvea X402 API
  slug: melvea-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/melvea-com/openapi/melvea-com-x402-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: melvea.com
  spf: false
hosts:
- cert_expires: Feb  5 06:09:08 2027 GMT
  host: melvea.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Melvea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Melvea, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Melvea
provider_slug: melvea-com
slug: melvea-com-domain-security
source_filename: melvea-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: melvea.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 06:09:08 2027 GMT\n  hsts: false\ndomains:\n- domain: melvea.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/melvea-com/security/melvea-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Honey
- Food
- Media
- Data
- Consumer
---
