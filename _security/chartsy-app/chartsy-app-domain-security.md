---
api_specs:
- filename: chartsy-app-openapi-generated.yml
  format: yaml
  label: Chartsy API
  slug: chartsy-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chartsy-app/openapi/_ae-authored/chartsy-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chartsy.app
  spf: true
hosts:
- cert_expires: Jan  2 17:18:22 2027 GMT
  host: chartsy.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chartsy App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chartsy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chartsy
provider_slug: chartsy-app
slug: chartsy-app-domain-security
source_filename: chartsy-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chartsy.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 17:18:22 2027 GMT\n  hsts: false\ndomains:\n- domain: chartsy.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/chartsy-app/security/chartsy-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Software-as-a-Service
- Analytics
- Revenue
- MRR
- Marketing
---
