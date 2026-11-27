---
api_specs:
- filename: monolithos-ai-openapi-generated.yml
  format: yaml
  label: Monolithos API
  slug: monolithos-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monolithos-ai/openapi/_ae-authored/monolithos-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: monolithos.ai
  spf: true
hosts:
- cert_expires: Jan 28 16:02:24 2027 GMT
  host: monolithos.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Monolithos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monolithos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Monolithos
provider_slug: monolithos-ai
slug: monolithos-ai-domain-security
source_filename: monolithos-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monolithos.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 16:02:24 2027 GMT\n  hsts: false\ndomains:\n- domain: monolithos.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/monolithos-ai/security/monolithos-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Personal Agent
- Enterprise Tools
- Cross-Platform
---
