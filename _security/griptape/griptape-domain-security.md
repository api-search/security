---
api_specs:
- filename: griptape-openapi-generated.yml
  format: yaml
  label: Foundry API
  slug: griptape-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/griptape/openapi/_ae-authored/griptape-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: griptape.ai
  spf: true
hosts:
- cert_expires: Dec 16 15:48:45 2026 GMT
  host: griptape.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Griptape Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Foundry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Foundry
provider_slug: griptape
slug: griptape-domain-security
source_filename: griptape-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: griptape.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 15:48:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: griptape.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/griptape/security/griptape-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Platform
- Workflow
- Automation
- OpenSource
---
