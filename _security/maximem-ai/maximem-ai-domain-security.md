---
api_specs:
- filename: maximem-ai-openapi-generated.yml
  format: yaml
  label: Maximem API
  slug: maximem-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/maximem-ai/openapi/_ae-authored/maximem-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: maximem.ai
  spf: true
hosts:
- cert_expires: Dec 23 00:02:53 2026 GMT
  host: maximem.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Maximem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maximem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Maximem
provider_slug: maximem-ai
slug: maximem-ai-domain-security
source_filename: maximem-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maximem.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 00:02:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: maximem.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/maximem-ai/security/maximem-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Memory
- Agent Memory
- Context Management
- Personal AI Memory
---
