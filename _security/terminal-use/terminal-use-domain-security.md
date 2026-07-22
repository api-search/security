---
api_specs:
- filename: terminal-use-openapi-original.json
  format: json
  label: Terminal Use API
  slug: terminal-use-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terminal-use/refs/heads/main/openapi/terminal-use-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: terminaluse.com
  spf: true
hosts:
- cert_expires: Oct 14 05:00:16 2026 GMT
  host: www.terminaluse.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 19:26:40 2026 GMT
  host: app.terminaluse.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 21:03:39 2026 GMT
  host: docs.terminaluse.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terminal Use Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Terminal Use, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Terminal Use
provider_slug: terminal-use
slug: terminal-use-domain-security
source_filename: terminal-use-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.terminaluse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 05:00:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.terminaluse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:26:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.terminaluse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 21:03:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: terminaluse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terminal-use/refs/heads/main/security/terminal-use-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agents
- AI Agents
- Background Agents
- Agent Infrastructure
- Deployment
- Orchestration
- Sandboxed Compute
- Filesystems
- Developer Tools
- SDK
- CLI
---
