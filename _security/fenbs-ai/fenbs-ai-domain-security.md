---
api_specs:
- filename: fenbs-ai-openapi-generated.yml
  format: yaml
  label: fenbs API
  slug: fenbs-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fenbs-ai/openapi/_ae-authored/fenbs-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: fenbs.ai
  spf: true
hosts:
- cert_expires: Jan 19 20:35:34 2027 GMT
  host: fenbs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: fenbs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fenbs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: fenbs
provider_slug: fenbs-ai
slug: fenbs-ai-domain-security
source_filename: fenbs-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fenbs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 20:35:34 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fenbs.ai\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fenbs-ai/security/fenbs-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Collaboration
- Project Management
- Kanban
- Productivity
---
