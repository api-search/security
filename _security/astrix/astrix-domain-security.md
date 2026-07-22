---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: astrix.security
  spf: true
hosts:
- cert_expires: Sep 13 10:42:24 2026 GMT
  host: astrix.security
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astrix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Astrix
provider_slug: astrix
slug: astrix-domain-security
source_filename: astrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astrix.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 10:42:24 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: astrix.security\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astrix/refs/heads/main/security/astrix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Non-Human Identity
- Identity Security
- AI Agent Security
- ITDR
- Secrets Management
- OAuth
- MCP Security
---
