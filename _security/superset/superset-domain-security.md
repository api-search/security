---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: superset.sh
  spf: true
hosts:
- cert_expires: Sep 25 03:58:53 2026 GMT
  host: superset.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 02:13:08 2026 GMT
  host: docs.superset.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 06:55:22 2026 GMT
  host: api.superset.sh
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superset Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superset, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Superset
provider_slug: superset
slug: superset-domain-security
source_filename: superset-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superset.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 03:58:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.superset.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 02:13:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.superset.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 06:55:22 2026 GMT\n  hsts: null\ndomains:\n- domain: superset.sh\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superset/refs/heads/main/security/superset-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- AI Agents
- Code Editor
- IDE
- Coding Agents
- MCP
- CLI
- SDK
- Git Worktrees
- Automation
- Y Combinator
---
