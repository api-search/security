---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jakegaylor.com
  spf: false
hosts:
- cert_expires: Nov  7 08:16:49 2026 GMT
  host: jakegaylor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 02:38:48 2026 GMT
  host: ai.jakegaylor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Jakegaylor Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jake Gaylor, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Jake Gaylor
provider_slug: jakegaylor-com
slug: jakegaylor-com-domain-security
source_filename: jakegaylor-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jakegaylor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 08:16:49 2026 GMT\n  hsts: false\n- host: ai.jakegaylor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 02:38:48 2026 GMT\n  hsts: false\ndomains:\n- domain: jakegaylor.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jakegaylor-com/refs/heads/main/security/jakegaylor-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Agents
- AI Agents
- A2A
- MCP
- Hiring
- Recruiting
- Resume
- Scheduling
- Personal Agent
---
