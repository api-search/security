---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: conteller.com
  spf: true
hosts:
- cert_expires: Aug 25 14:41:51 2026 GMT
  host: conteller.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conteller Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conteller, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Conteller
provider_slug: conteller
slug: conteller-domain-security
source_filename: conteller-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conteller.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 14:41:51 2026 GMT\n  hsts: null\ndomains:\n- domain: conteller.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conteller/refs/heads/main/security/conteller-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- User Generated Content
- Content Marketing
- Creator Economy
- Marketing
- Media
- Startup
---
