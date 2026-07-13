---
api_specs:
- filename: jentic-openapi.yml
  format: yaml
  label: Jentic API
  slug: jentic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jentic/refs/heads/main/openapi/jentic-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jentic.com
  spf: true
hosts:
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: jentic.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: docs.jentic.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: api.jentic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jentic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jentic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jentic
provider_slug: jentic
slug: jentic-domain-security
source_filename: jentic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jentic.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: false\n- host: docs.jentic.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: false\n- host: api.jentic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: jentic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jentic/refs/heads/main/security/jentic-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- AI Agents
- Arazzo
- OpenAPI
- MCP
- Workflows
- Integrations
- Agent Runtime
- Standard Agent
- Just In Time Tooling
- Credential Vault
- Agent Governance
- Observability
- API AI Readiness
---
