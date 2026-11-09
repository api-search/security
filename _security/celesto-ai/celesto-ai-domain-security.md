---
api_specs:
- filename: celesto-ai-agentor-openapi-generated.yml
  format: yaml
  label: Celesto AI agentor API
  slug: agentor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/celesto-ai/openapi/_ae-authored/celesto-ai-agentor-openapi-generated.yml
- filename: celesto-ai-celesto-openapi-generated.yml
  format: yaml
  label: Celesto AI celesto API
  slug: celesto-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/celesto-ai/openapi/_ae-authored/celesto-ai-celesto-openapi-generated.yml
- filename: celesto-ai-core-openapi-generated.yml
  format: yaml
  label: Celesto AI core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/celesto-ai/openapi/_ae-authored/celesto-ai-core-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: celesto.ai
  spf: true
hosts:
- cert_expires: Dec 13 19:40:57 2026 GMT
  host: celesto.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Celesto Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celesto AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Celesto AI
provider_slug: celesto-ai
slug: celesto-ai-domain-security
source_filename: celesto-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: celesto.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 19:40:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: celesto.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/celesto-ai/security/celesto-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- CI
- Runners
- Cloud
- Automation
- Company
---
