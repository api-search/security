---
api_specs:
- filename: fluxsocial-app-openapi-generated.yml
  format: yaml
  label: FluxSocial API
  slug: fluxsocial-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxsocial-app/openapi/_ae-authored/fluxsocial-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fluxsocial.app
  spf: true
hosts:
- cert_expires: Jan 14 10:55:16 2027 GMT
  host: fluxsocial.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FluxSocial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FluxSocial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FluxSocial
provider_slug: fluxsocial-app
slug: fluxsocial-app-domain-security
source_filename: fluxsocial-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fluxsocial.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 10:55:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fluxsocial.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fluxsocial-app/security/fluxsocial-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Social Media
- Video Generation
- Marketing
- Automation
---
