---
api_specs:
- filename: needhuman-ai-openapi-generated.yml
  format: yaml
  label: needhuman-ai API
  slug: needhuman-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/needhuman-ai/openapi/_ae-authored/needhuman-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: needhuman.ai
  spf: true
hosts:
- cert_expires: Jan 23 14:38:54 2027 GMT
  host: needhuman.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Needhuman Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for needhuman-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: needhuman-ai
provider_slug: needhuman-ai
slug: needhuman-ai-domain-security
source_filename: needhuman-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: needhuman.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 14:38:54 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: needhuman.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/needhuman-ai/security/needhuman-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Human-in-the-loop
- Platform
- Automation
---
