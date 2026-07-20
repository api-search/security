---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ctd.ai
  spf: true
hosts:
- cert_expires: Aug 27 21:42:26 2026 GMT
  host: ctd.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ctd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connect The Dots, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Connect The Dots
provider_slug: ctd
slug: ctd-domain-security
source_filename: ctd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ctd.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 21:42:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: ctd.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ctd/refs/heads/main/security/ctd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Relationship Intelligence
- Sales
- Warm Introductions
- Network Graph
- CRM
- MCP
- Venture Capital
---
