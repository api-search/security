---
api_specs:
- filename: octocrawl-dev-openapi-generated.yml
  format: yaml
  label: octocrawl-dev API
  slug: octocrawl-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/octocrawl-dev/openapi/_ae-authored/octocrawl-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: octocrawl.dev
  spf: true
hosts:
- cert_expires: Jan  4 08:49:12 2027 GMT
  host: octocrawl.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Octocrawl Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for octocrawl-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: octocrawl-dev
provider_slug: octocrawl-dev
slug: octocrawl-dev-domain-security
source_filename: octocrawl-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: octocrawl.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 08:49:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: octocrawl.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/octocrawl-dev/security/octocrawl-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- API
- WebScraping
- DataExtraction
- SaaS
- Automation
---
