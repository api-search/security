---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: polimorphic.com
  spf: true
hosts:
- cert_expires: Sep  9 16:18:36 2026 GMT
  host: www.polimorphic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polimorphic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polimorphic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Polimorphic
provider_slug: polimorphic
slug: polimorphic-domain-security
source_filename: polimorphic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.polimorphic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 16:18:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: polimorphic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polimorphic/refs/heads/main/security/polimorphic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- GovTech
- Government
- Artificial Intelligence
- CRM
- Workflows
- Public Sector
- Constituent Services
- Voice AI
- Chatbot
---
