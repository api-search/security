---
api_specs:
- filename: factory-automations-api-openapi.yml
  format: yaml
  label: Factory Automations API
  slug: factory-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/factory/openapi/factory-automations-api-openapi.yml
- filename: factory-computers-api-openapi.yml
  format: yaml
  label: Factory Computers API
  slug: factory-computers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/factory/openapi/factory-computers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: factory.com
  spf: true
hosts:
- cert_expires: Jan 16 02:31:21 2027 GMT
  host: factory.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Factory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Factory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Factory
provider_slug: factory
slug: factory-domain-security
source_filename: factory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: factory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 02:31:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: factory.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/factory/security/factory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Manufacturing
- SaaS
- Cloud
- Automation
- Supply-Chain
- Company
---
