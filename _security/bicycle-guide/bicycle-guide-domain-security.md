---
api_specs:
- filename: bicycle-guide-guide-registry-api-openapi.yml
  format: yaml
  label: Bicycle Guide Guide Registry API
  slug: bicycle-guide-guide-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bicycle-guide/openapi/bicycle-guide-guide-registry-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bicycle.guide
  spf: false
hosts:
- cert_expires: Jan 19 18:46:12 2027 GMT
  host: bicycle.guide
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bicycle Guide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bicycle Guide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Bicycle Guide
provider_slug: bicycle-guide
slug: bicycle-guide-domain-security
source_filename: bicycle-guide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bicycle.guide\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 18:46:12 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bicycle.guide\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bicycle-guide/security/bicycle-guide-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Guides
- Artificial Intelligence
- Education
- Library
---
