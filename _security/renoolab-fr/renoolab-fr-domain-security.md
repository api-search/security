---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: renoolab.fr
  spf: true
hosts:
- cert_expires: Nov 27 12:45:12 2026 GMT
  host: renoolab.fr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Renoolab Fr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RenooLab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RenooLab
provider_slug: renoolab-fr
slug: renoolab-fr-domain-security
source_filename: renoolab-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: renoolab.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 12:45:12 2026 GMT\n  hsts: false\ndomains:\n- domain: renoolab.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/renoolab-fr/refs/heads/main/security/renoolab-fr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Home Services
- Construction
- Building Trades
- Renovation
- Marketplace
- Local Services
- MCP
- A2A
- AI Agents
- Agent Skills
- France
---
