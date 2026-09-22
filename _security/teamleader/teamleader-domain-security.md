---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: teamleader.eu
  spf: true
hosts:
- cert_expires: Nov 20 23:40:13 2026 GMT
  host: teamleader.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Teamleader Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teamleader, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Teamleader
provider_slug: teamleader
slug: teamleader-domain-security
source_filename: teamleader-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teamleader.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:40:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: teamleader.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teamleader/refs/heads/main/security/teamleader-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CRM
- Invoicing
- Project Management
- SaaS
- SME
---
