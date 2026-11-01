---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uctomost.sk
  spf: true
hosts:
- cert_expires: Dec  5 12:54:42 2026 GMT
  host: uctomost.sk
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Uctomost Sk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for uctomost-sk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: uctomost-sk
provider_slug: uctomost-sk
slug: uctomost-sk-domain-security
source_filename: uctomost-sk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uctomost.sk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 12:54:42 2026 GMT\n  hsts: false\ndomains:\n- domain: uctomost.sk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/uctomost-sk/security/uctomost-sk-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Accounting
- Automation
- FinTech
- Slovakia
---
