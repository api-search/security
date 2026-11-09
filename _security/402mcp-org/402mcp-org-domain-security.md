---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: 402mcp.org
  spf: true
hosts:
- cert_expires: Dec 20 14:10:03 2026 GMT
  host: 402mcp.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 402Mcp Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 402MCP.org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 402MCP.org
provider_slug: 402mcp-org
slug: 402mcp-org-domain-security
source_filename: 402mcp-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 402mcp.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 14:10:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 402mcp.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/402mcp-org/security/402mcp-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Artificial Intelligence
- Agents
- Registry
- OpenAPI
---
