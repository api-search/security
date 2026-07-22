---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: metorial.com
  spf: true
hosts:
- cert_expires: Oct 14 09:14:45 2026 GMT
  host: metorial.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 17:35:19 2026 GMT
  host: api.metorial.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metorial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metorial, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Metorial
provider_slug: metorial
slug: metorial-domain-security
source_filename: metorial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metorial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 09:14:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.metorial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 17:35:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: metorial.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metorial/refs/heads/main/security/metorial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- MCP
- Model Context Protocol
- AI Agents
- Agentic Infrastructure
- Integrations
- Developer Tools
- Serverless
- API
---
