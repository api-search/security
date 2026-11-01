---
api_specs:
- filename: middle-openapi-generated.yml
  format: yaml
  label: Middle API
  slug: middle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/middle/openapi/_ae-authored/middle-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: middle.app
  spf: true
hosts:
- cert_expires: Jan 11 22:23:25 2027 GMT
  host: middle.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Middle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Middle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Middle
provider_slug: middle
slug: middle-domain-security
source_filename: middle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: middle.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 22:23:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: middle.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/middle/security/middle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Integration Platform
- iPaaS
- Data Integration
---
