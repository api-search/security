---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: geordie.ai
  spf: true
hosts:
- cert_expires: Aug 26 07:04:24 2026 GMT
  host: www.geordie.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geordie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geordie AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Geordie AI
provider_slug: geordie
slug: geordie-domain-security
source_filename: geordie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.geordie.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 07:04:24 2026 GMT\n  hsts: false\ndomains:\n- domain: geordie.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geordie/refs/heads/main/security/geordie-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI Governance
- AI Agents
- Agentic AI
- AI Security
- Observability
- Compliance
- Enterprise Security
- MCP
---
