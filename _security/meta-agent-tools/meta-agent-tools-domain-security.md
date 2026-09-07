---
api_specs:
- filename: openapi.json
  format: json
  label: Meta Agent Tools API
  slug: meta-agent-tools-api
  spec_type: OpenAPI
  url: https://agentalog.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: classificado.app.br
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentalog.com
  spf: true
hosts:
- cert_expires: Nov 16 17:42:23 2026 GMT
  host: classificado.app.br
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 16:31:06 2026 GMT
  host: agentalog.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Meta Agent Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meta Agent Tools, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Meta Agent Tools
provider_slug: meta-agent-tools
slug: meta-agent-tools-domain-security
source_filename: meta-agent-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: classificado.app.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 17:42:23 2026 GMT\n  hsts: false\n- host: agentalog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 16:31:06 2026 GMT\n  hsts: false\ndomains:\n- domain: classificado.app.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: agentalog.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meta-agent-tools/refs/heads/main/security/meta-agent-tools-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Developer Tools
- API Registry
- Agent Registry
- MCP
- Agent Skills
- AI Agents
- Catalog
- Directory
- Search & Discovery
- x402
- Agent Payments
- Community
- UGC
---
