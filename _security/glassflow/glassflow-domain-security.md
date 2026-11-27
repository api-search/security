---
api_specs:
- filename: glassflow-openapi-generated.yml
  format: yaml
  label: GlassFlow API
  slug: glassflow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glassflow/openapi/_ae-authored/glassflow-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: glassflow.ai
  spf: true
hosts:
- cert_expires: Jan 21 15:52:51 2027 GMT
  host: glassflow.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GlassFlow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GlassFlow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: GlassFlow
provider_slug: glassflow
slug: glassflow-domain-security
source_filename: glassflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glassflow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 15:52:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: glassflow.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/glassflow/security/glassflow-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Observability
- Data Infrastructure
- Agents
---
