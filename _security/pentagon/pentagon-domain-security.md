---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pentagon.run
  spf: true
hosts:
- cert_expires: Oct 17 11:20:02 2026 GMT
  host: pentagon.run
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pentagon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pentagon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pentagon
provider_slug: pentagon
slug: pentagon-domain-security
source_filename: pentagon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pentagon.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 11:20:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: pentagon.run\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pentagon/refs/heads/main/security/pentagon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agent Orchestration
- Multi-Agent Systems
- Developer Tools
- Productivity
- Workspace
- Y Combinator
---
