---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: conceptdrop.com
  spf: true
hosts:
- cert_expires: Sep 25 14:48:57 2026 GMT
  host: conceptdrop.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexus Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexus AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nexus AI
provider_slug: nexus-ai
slug: nexus-ai-domain-security
source_filename: nexus-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conceptdrop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:48:57 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: conceptdrop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexus-ai/refs/heads/main/security/nexus-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Freelance
- Talent Marketplace
- Creative Services
- Staffing
- Outsourcing
- Design
---
