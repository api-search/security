---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: genspark.ai
  spf: true
hosts:
- cert_expires: Aug 29 01:14:53 2026 GMT
  host: www.genspark.ai
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genspark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genspark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Genspark
provider_slug: genspark
slug: genspark-domain-security
source_filename: genspark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.genspark.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 01:14:53 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: genspark.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genspark/refs/heads/main/security/genspark-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Artificial Intelligence
- AI Agents
- MCP
- Model Context Protocol
- Productivity
- Automation
- Search
- Workspace
---
