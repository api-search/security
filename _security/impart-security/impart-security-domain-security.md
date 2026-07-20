---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: impart.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: impartsecurity.net
  spf: false
hosts:
- cert_expires: Sep 21 01:14:47 2026 GMT
  host: www.impart.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 23:59:59 2026 GMT
  host: docs.impartsecurity.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.impartsecurity.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Impart Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Impart Security, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Impart Security
provider_slug: impart-security
slug: impart-security-domain-security
source_filename: impart-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.impart.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 01:14:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.impartsecurity.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 23:59:59 2026 GMT\n  hsts: null\n- host: api.impartsecurity.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: impart.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: impartsecurity.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impart-security/refs/heads/main/security/impart-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- API Security
- Runtime Protection
- WAF
- LLM Security
- AI Security
- MCP
- Agent Security
- Kong
- Governance
---
