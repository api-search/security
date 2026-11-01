---
api_specs:
- filename: registrum-co-uk-openapi.json
  format: json
  label: Registrum API
  slug: registrum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/registrum-co-uk/openapi/registrum-co-uk-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: registrum.co.uk
  spf: true
hosts:
- cert_expires: Nov 29 09:23:59 2026 GMT
  host: registrum.co.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Registrum Co Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for registrum-co-uk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: registrum-co-uk
provider_slug: registrum-co-uk
slug: registrum-co-uk-domain-security
source_filename: registrum-co-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: registrum.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 09:23:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: registrum.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/registrum-co-uk/security/registrum-co-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Companies House
- Financial Data
- JSON API
- UK
- Business Intelligence
---
