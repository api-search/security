---
api_specs:
- filename: golfdata-co-api-openapi.json
  format: json
  label: GolfDataAPI API
  slug: golfdataapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/golfdata-co/openapi/_original/golfdata-co-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: golfdata.co
  spf: true
hosts:
- cert_expires: Dec 15 18:37:18 2026 GMT
  host: golfdata.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GolfData Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GolfData, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GolfData
provider_slug: golfdata-co
slug: golfdata-co-domain-security
source_filename: golfdata-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: golfdata.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 18:37:18 2026 GMT\n  hsts: false\ndomains:\n- domain: golfdata.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/golfdata-co/security/golfdata-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Golf
- Data
- Pricing
- Equipment
---
