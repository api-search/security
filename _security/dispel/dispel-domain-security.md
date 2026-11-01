---
api_specs:
- filename: dispel-openapi-generated.yml
  format: yaml
  label: Dispel API
  slug: dispel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dispel/openapi/_ae-authored/dispel-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dispel.com
  spf: true
hosts:
- cert_expires: Jan  6 21:40:26 2027 GMT
  host: dispel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dispel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dispel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dispel
provider_slug: dispel
slug: dispel-domain-security
source_filename: dispel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dispel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 21:40:26 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dispel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dispel/security/dispel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- OT Security
- Industrial IoT
- Zero Trust
- Remote Access
- Data Streaming
---
