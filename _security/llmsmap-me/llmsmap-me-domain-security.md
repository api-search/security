---
api_specs:
- filename: llmsmap-me-directory-api-openapi.yml
  format: yaml
  label: llmsmap.me Directory API
  slug: llmsmap-me-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmsmap-me/openapi/llmsmap-me-directory-api-openapi.yml
- filename: llmsmap-me-submissions-api-openapi.yml
  format: yaml
  label: llmsmap.me Submissions API
  slug: llmsmap-me-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/llmsmap-me/openapi/llmsmap-me-submissions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: llmsmap.me
  spf: true
hosts:
- cert_expires: Feb  1 06:54:09 2027 GMT
  host: llmsmap.me
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: llmsmap.me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for llmsmap.me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: llmsmap.me
provider_slug: llmsmap-me
slug: llmsmap-me-domain-security
source_filename: llmsmap-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: llmsmap.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 06:54:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: llmsmap.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/llmsmap-me/security/llmsmap-me-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Directory
- AI-Readiness
- Llms.txt
- Llms Full.txt
- Generators
- Crawlers
---
