---
api_specs:
- filename: machinerealms-com-research-commons-openapi.json
  format: json
  label: Machine Realms Research Commons API
  slug: research-commons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/machinerealms-com/refs/heads/main/openapi/machinerealms-com-research-commons-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: machinerealms.com
  spf: true
hosts:
- cert_expires: Dec  7 00:52:01 2026 GMT
  host: machinerealms.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Machinerealms Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Machine Realms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Machine Realms
provider_slug: machinerealms-com
slug: machinerealms-com-domain-security
source_filename: machinerealms-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: machinerealms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 00:52:01 2026 GMT\n  hsts: null\ndomains:\n- domain: machinerealms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/machinerealms-com/refs/heads/main/security/machinerealms-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Agents
- A2A
- MCP
- Research
- Agent Discovery
- Machine Web
- Registry
- Evidence
- Research Commons
- agent-native
---
