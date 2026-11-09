---
api_specs:
- filename: e-esim-com-openapi.json
  format: json
  label: e-eSIM Catalog API
  slug: e-esim-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/e-esim-com/openapi/e-esim-com-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: e-esim.com
  spf: true
hosts:
- cert_expires: Dec 31 16:32:58 2026 GMT
  host: e-esim.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: E Esim Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IbiPoint Ltd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: IbiPoint Ltd
provider_slug: e-esim-com
slug: e-esim-com-domain-security
source_filename: e-esim-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: e-esim.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 16:32:58 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: e-esim.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/e-esim-com/security/e-esim-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- eSIM
- Travel Data
- Prepaid Mobile
- Mobile Data
---
