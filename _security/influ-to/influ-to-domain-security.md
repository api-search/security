---
api_specs:
- filename: influ-to-openapi-generated.yml
  format: yaml
  label: InfluTo API
  slug: influ-to-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/influ-to/openapi/_ae-authored/influ-to-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: influ.to
  spf: true
hosts:
- cert_expires: Jan  2 14:41:09 2027 GMT
  host: influ.to
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: InfluTo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InfluTo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: InfluTo
provider_slug: influ-to
slug: influ-to-domain-security
source_filename: influ-to-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: influ.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 14:41:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: influ.to\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/influ-to/security/influ-to-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Affiliates
- Mobile
- iOS
- Android
- Marketing
---
