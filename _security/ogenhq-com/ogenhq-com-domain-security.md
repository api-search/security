---
api_specs:
- filename: ogenhq-com-rest-api-openapi.yml
  format: yaml
  label: Ogen Rest API
  slug: ogenhq-com-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ogenhq-com/openapi/ogenhq-com-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ogenhq.com
  spf: false
hosts:
- cert_expires: Feb  4 07:04:28 2027 GMT
  host: ogenhq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ogen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ogen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Ogen
provider_slug: ogenhq-com
slug: ogenhq-com-domain-security
source_filename: ogenhq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ogenhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 07:04:28 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ogenhq.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ogenhq-com/security/ogenhq-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Automation
- Workflows
- Compliance
- Data Integration
---
