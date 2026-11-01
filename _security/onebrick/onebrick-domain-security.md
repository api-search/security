---
api_specs:
- filename: onebrick-openapi-generated.yml
  format: yaml
  label: Brick API
  slug: onebrick-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onebrick/openapi/_ae-authored/onebrick-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: onebrick.io
  spf: true
hosts:
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: onebrick.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Onebrick Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brick, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Brick
provider_slug: onebrick
slug: onebrick-domain-security
source_filename: onebrick-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onebrick.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: onebrick.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/onebrick/security/onebrick-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Fintech
- Payments
- Southeast Asia
- B2B
---
