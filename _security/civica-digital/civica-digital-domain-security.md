---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: civica.digital
  spf: true
hosts:
- cert_expires: Sep 30 00:15:25 2026 GMT
  host: civica.digital
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Civica Digital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Civica Digital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Civica Digital
provider_slug: civica-digital
slug: civica-digital-domain-security
source_filename: civica-digital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: civica.digital\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 00:15:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: civica.digital\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/civica-digital/refs/heads/main/security/civica-digital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Civic Technology
- Digital Government
- Public Sector
- GovTech
- Digital Transformation
- Document Management
- Conversational AI
- Mexico
---
