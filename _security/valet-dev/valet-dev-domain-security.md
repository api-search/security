---
api_specs:
- filename: valet-dev-install-api-openapi.yml
  format: yaml
  label: valet-dev Install API
  slug: valet-dev-install-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valet-dev/openapi/valet-dev-install-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: valet.dev
  spf: true
hosts:
- cert_expires: May 10 23:59:59 2027 GMT
  host: valet.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: valet-dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for valet-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: valet-dev
provider_slug: valet-dev
slug: valet-dev-domain-security
source_filename: valet-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: valet.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: valet.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/valet-dev/security/valet-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Platform
- Citizen-Developer
- Automation
- Integration
---
