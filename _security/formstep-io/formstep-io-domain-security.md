---
api_specs:
- filename: formstep-io-methods-api-openapi.yml
  format: yaml
  label: Formstep Methods API
  slug: formstep-io-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formstep-io/openapi/formstep-io-methods-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: formstep.io
  spf: true
hosts:
- cert_expires: Jan  5 19:05:08 2027 GMT
  host: formstep.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Formstep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Formstep, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Formstep
provider_slug: formstep-io
slug: formstep-io-domain-security
source_filename: formstep-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: formstep.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 19:05:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: formstep.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/formstep-io/security/formstep-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Forms
- Automation
- Data Collection
- Workflow Integration
- Software-as-a-Service
---
