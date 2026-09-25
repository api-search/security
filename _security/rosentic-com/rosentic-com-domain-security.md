---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rosentic.com
  spf: true
hosts:
- cert_expires: Dec  4 05:30:57 2026 GMT
  host: rosentic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  9 12:40:51 2026 GMT
  host: api.rosentic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Rosentic Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rosentic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rosentic
provider_slug: rosentic-com
slug: rosentic-com-domain-security
source_filename: rosentic-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rosentic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 05:30:57 2026 GMT\n  hsts: false\n- host: api.rosentic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 12:40:51 2026 GMT\n  hsts: false\ndomains:\n- domain: rosentic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rosentic-com/refs/heads/main/security/rosentic-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Developer Tools
- CI/CD
- Git
- Static Analysis
- Merge Safety
- AI Coding Agents
- MCP
- A2A
- GitHub Actions
- Agent-Native
---
