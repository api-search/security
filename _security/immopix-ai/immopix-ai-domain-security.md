---
api_specs:
- filename: immopix-ai-openapi-generated.yml
  format: yaml
  label: Immopix API
  slug: immopix-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/immopix-ai/openapi/_ae-authored/immopix-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: immopix.ai
  spf: true
hosts:
- cert_expires: Jan 23 17:47:50 2027 GMT
  host: immopix.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Immopix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Immopix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Immopix
provider_slug: immopix-ai
slug: immopix-ai-domain-security
source_filename: immopix-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: immopix.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 17:47:50 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: immopix.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/immopix-ai/security/immopix-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
