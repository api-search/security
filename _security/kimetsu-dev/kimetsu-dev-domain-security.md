---
api_specs:
- filename: kimetsu-dev-agent-gateway-openapi.yml
  format: yaml
  label: kimetsu.dev Agent Gateway
  slug: agent-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kimetsu-dev/refs/heads/main/openapi/kimetsu-dev-agent-gateway-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: kimetsu.dev
  spf: true
hosts:
- cert_expires: Nov 21 04:05:39 2026 GMT
  host: kimetsu.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 03:19:14 2026 GMT
  host: agents.kimetsu.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Kimetsu Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kimetsu, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Kimetsu
provider_slug: kimetsu-dev
slug: kimetsu-dev-domain-security
source_filename: kimetsu-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kimetsu.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 04:05:39 2026 GMT\n  hsts: false\n- host: agents.kimetsu.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 03:19:14 2026 GMT\n  hsts: false\ndomains:\n- domain: kimetsu.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kimetsu-dev/refs/heads/main/security/kimetsu-dev-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- AI Agents
- Agent Memory
- Coding Agents
- MCP
- A2A
- Developer Tools
- Open Source
- Rust
- Agent Discovery
- Public Goods
---
