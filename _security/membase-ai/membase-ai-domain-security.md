---
api_specs:
- filename: membase-ai-agent-protocol-api-openapi.yml
  format: yaml
  label: Membase Agent Protocol API
  slug: membase-ai-agent-protocol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/membase-ai/openapi/membase-ai-agent-protocol-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: membase.ai
  spf: true
hosts:
- cert_expires: Apr 25 10:06:54 2027 GMT
  host: membase.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Membase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Membase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Membase
provider_slug: membase-ai
slug: membase-ai-domain-security
source_filename: membase-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: membase.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 25 10:06:54 2027 GMT\n  hsts: false\ndomains:\n- domain: membase.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/membase-ai/security/membase-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Memory
- Platform
- Developer Tools
- Unibase
---
