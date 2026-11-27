---
api_specs:
- filename: butterbase-ai-openapi-generated.yml
  format: yaml
  label: Butterbase API
  slug: butterbase-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/butterbase-ai/openapi/_ae-authored/butterbase-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: butterbase.ai
  spf: false
hosts:
- cert_expires: Dec 27 16:15:40 2026 GMT
  host: butterbase.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Butterbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Butterbase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Butterbase
provider_slug: butterbase-ai
slug: butterbase-ai-domain-security
source_filename: butterbase-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: butterbase.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 16:15:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: butterbase.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/butterbase-ai/security/butterbase-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Backend
- Business
- Agent-Native
- Platform
---
