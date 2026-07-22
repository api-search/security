---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: entire.io
  spf: true
hosts:
- cert_expires: Oct  3 16:12:47 2026 GMT
  host: entire.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Entire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Entire
provider_slug: entire
slug: entire-domain-security
source_filename: entire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: entire.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 16:12:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: entire.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entire/refs/heads/main/security/entire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Developer Tools
- Developer Platform
- Git
- Git Hosting
- Version Control
- Source Control
- AI Agents
- Agent Infrastructure
- CLI
---
