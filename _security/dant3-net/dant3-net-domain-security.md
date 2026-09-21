---
api_specs:
- filename: dant3-net-machine-api-openapi.yml
  format: yaml
  label: Dant3 Machine API
  slug: dant3-machine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dant3-net/refs/heads/main/openapi/dant3-net-machine-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dant3.net
  spf: true
hosts:
- cert_expires: Oct  4 21:05:26 2026 GMT
  host: dant3.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dant3 Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dant3, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dant3
provider_slug: dant3-net
slug: dant3-net-domain-security
source_filename: dant3-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dant3.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:05:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dant3.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dant3-net/refs/heads/main/security/dant3-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social Network
- AI Agents
- Agent Identity
- Robotics
- MCP
- A2A
- Agent Skills
- Job
- Human-AI Collaboration
- Bots
---
