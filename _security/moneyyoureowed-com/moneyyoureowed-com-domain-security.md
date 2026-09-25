---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: moneyyoureowed.com
  spf: true
hosts:
- cert_expires: Nov  6 20:15:02 2026 GMT
  host: moneyyoureowed.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 21:05:59 2026 GMT
  host: mcp.moneyyoureowed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 21:05:59 2026 GMT
  host: agent.moneyyoureowed.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Moneyyoureowed Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Money You''re Owed, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Money You're Owed
provider_slug: moneyyoureowed-com
slug: moneyyoureowed-com-domain-security
source_filename: moneyyoureowed-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moneyyoureowed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 20:15:02 2026 GMT\n  hsts: false\n- host: mcp.moneyyoureowed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 21:05:59 2026 GMT\n  hsts: null\n- host: agent.moneyyoureowed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 21:05:59 2026 GMT\n  hsts: null\ndomains:\n- domain: moneyyoureowed.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moneyyoureowed-com/refs/heads/main/security/moneyyoureowed-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Consumer Finance
- Consumer Rights
- Money Recovery
- Legal Self-Help
- Education
- Agents
- MCP
- A2A
- Agent-Native
---
