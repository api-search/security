---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getelva.ai
  spf: false
hosts:
- cert_expires: Dec  2 15:38:23 2026 GMT
  host: docs.getelva.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 12:50:26 2026 GMT
  host: api.getelva.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Elva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elva, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Elva
provider_slug: elva
slug: elva-domain-security
source_filename: elva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.getelva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 15:38:23 2026 GMT\n  hsts: null\n- host: api.getelva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 12:50:26 2026 GMT\n  hsts: null\ndomains:\n- domain: getelva.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elva/refs/heads/main/security/elva-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Management
- MCP Server
- MCP Logs
- MCP Insights
- API Client
- API Contract
- API Governance
- API Discovery
- OpenAPI
- API Testing
- Developer Tools
- AI Agent Infrastructure
---
