---
api_specs:
- filename: lenshub-ai-openapi-generated.yml
  format: yaml
  label: LensHub API
  slug: lenshub-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenshub-ai/openapi/_ae-authored/lenshub-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lenshub.ai
  spf: true
hosts:
- cert_expires: Feb  7 00:05:07 2027 GMT
  host: lenshub.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LensHub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LensHub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LensHub
provider_slug: lenshub-ai
slug: lenshub-ai-domain-security
source_filename: lenshub-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lenshub.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 00:05:07 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lenshub.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lenshub-ai/security/lenshub-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Knowledge Management
- Enterprise Software
- Integration
- Automation
---
