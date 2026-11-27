---
api_specs:
- filename: humandesignhub-app-openapi-generated.yml
  format: yaml
  label: Human Design Hub API
  slug: humandesignhub-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/humandesignhub-app/openapi/_ae-authored/humandesignhub-app-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: humandesignhub.app
  spf: true
hosts:
- cert_expires: Jan 14 14:06:23 2027 GMT
  host: humandesignhub.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Human Design Hub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Human Design Hub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Human Design Hub
provider_slug: humandesignhub-app
slug: humandesignhub-app-domain-security
source_filename: humandesignhub-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humandesignhub.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 14:06:23 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: humandesignhub.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/humandesignhub-app/security/humandesignhub-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Human Design
- Charts
- Astrology
- Personal Development
---
