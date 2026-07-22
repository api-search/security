---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: commandbar.com
  spf: true
hosts:
- cert_expires: Oct  1 22:44:12 2026 GMT
  host: www.commandbar.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Commandbar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for commandbar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: commandbar
provider_slug: commandbar
slug: commandbar-domain-security
source_filename: commandbar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.commandbar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 22:44:12 2026 GMT\n  hsts: null\ndomains:\n- domain: commandbar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commandbar/refs/heads/main/security/commandbar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Product Adoption
- User Onboarding
- In-App Support
- Digital Adoption
- Customer Experience
- SaaS
---
