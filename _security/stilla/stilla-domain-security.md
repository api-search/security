---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stilla.ai
  spf: true
hosts:
- cert_expires: Oct  1 23:08:07 2026 GMT
  host: stilla.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 19:03:10 2026 GMT
  host: api.stilla.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stilla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stilla, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stilla
provider_slug: stilla
slug: stilla-domain-security
source_filename: stilla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stilla.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:08:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stilla.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:03:10 2026 GMT\n  hsts: null\ndomains:\n- domain: stilla.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stilla/refs/heads/main/security/stilla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agentic
- Productivity
- Collaboration
- MCP
- Automation
- Developer Tools
- Enterprise
---
