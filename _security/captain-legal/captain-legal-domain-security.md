---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: captain.legal
  spf: true
hosts:
- cert_expires: Dec  5 02:50:13 2026 GMT
  host: www.captain.legal
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Captain.Legal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Captain.Legal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Captain.Legal
provider_slug: captain-legal
slug: captain-legal-domain-security
source_filename: captain-legal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.captain.legal\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 02:50:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: captain.legal\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/captain-legal/security/captain-legal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Legal
- Legal Documents
- Contracts
- Templates
- Legal Tech
- MCP
- AI Assistant
---
