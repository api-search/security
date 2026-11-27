---
api_specs:
- filename: agoria-studio-search-api-openapi.yml
  format: yaml
  label: Agoria Search API
  slug: agoria-studio-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agoria-studio/openapi/agoria-studio-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: agoria.studio
  spf: true
hosts:
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: agoria.studio
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agoria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agoria, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Agoria
provider_slug: agoria-studio
slug: agoria-studio-domain-security
source_filename: agoria-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agoria.studio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agoria.studio\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/agoria-studio/security/agoria-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Business
- Platform
- Commerce
- Automation
---
