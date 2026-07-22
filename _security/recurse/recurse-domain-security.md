---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: recurse.ml
  spf: true
hosts:
- cert_expires: Oct  6 12:05:29 2026 GMT
  host: recurse.ml
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Recurse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recurse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Recurse
provider_slug: recurse
slug: recurse-domain-security
source_filename: recurse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: recurse.ml\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 12:05:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: recurse.ml\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recurse/refs/heads/main/security/recurse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Code Review
- Code Review
- Developer Tools
- CLI
- MCP
- AI Agents
- Static Analysis
- Bug Detection
- Code Quality
---
