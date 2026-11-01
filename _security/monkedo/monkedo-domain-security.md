---
api_specs:
- filename: monkedo-openapi-generated.yml
  format: yaml
  label: Z Yazilim API
  slug: monkedo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monkedo/openapi/_ae-authored/monkedo-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: monkedo.com
  spf: true
hosts:
- cert_expires: Dec 26 18:30:44 2026 GMT
  host: monkedo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Monkedo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Z Yazilim, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Z Yazilim
provider_slug: monkedo
slug: monkedo-domain-security
source_filename: monkedo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monkedo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 18:30:44 2026 GMT\n  hsts: false\ndomains:\n- domain: monkedo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/monkedo/security/monkedo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automation
- No-Code
- Integration
- Workflow
---
