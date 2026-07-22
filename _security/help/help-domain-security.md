---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: venturz.co
  spf: true
hosts:
- cert_expires: Sep  1 07:30:32 2026 GMT
  host: venturz.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Help Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HELP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HELP
provider_slug: help
slug: help-domain-security
source_filename: help-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: venturz.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 07:30:32 2026 GMT\n  hsts: false\ndomains:\n- domain: venturz.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/help/refs/heads/main/security/help-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Startups
- No-Code
- Business Operating System
- CRM
- Website Builder
- Founder Tools
- AI
---
