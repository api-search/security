---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: boltmcp.io
  spf: true
hosts:
- cert_expires: Nov  5 20:54:26 2026 GMT
  host: www.boltmcp.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 00:31:52 2026 GMT
  host: install.boltmcp.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Boltmcp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BoltMCP, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BoltMCP
provider_slug: boltmcp
slug: boltmcp-domain-security
source_filename: boltmcp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boltmcp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 20:54:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: install.boltmcp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 00:31:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: boltmcp.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boltmcp/refs/heads/main/security/boltmcp-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- MCP
- Agents
- Artificial Intelligence
- Kubernetes
- Self-Hosted
- Enterprise
- Identity
- Developer Tools
---
