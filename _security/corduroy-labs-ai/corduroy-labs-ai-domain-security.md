---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: corduroy-labs.ai
  spf: true
hosts:
- cert_expires: Dec 11 07:22:29 2026 GMT
  host: corduroy-labs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Corduroy Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corduroy Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Corduroy Labs
provider_slug: corduroy-labs-ai
slug: corduroy-labs-ai-domain-security
source_filename: corduroy-labs-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: corduroy-labs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 07:22:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: corduroy-labs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/corduroy-labs-ai/security/corduroy-labs-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agentic Operations
- MCP
- Agent Skills
- Open Source
- Workflow Automation
- Consulting
---
