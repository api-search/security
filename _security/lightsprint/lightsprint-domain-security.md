---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lightsprint.ai
  spf: true
hosts:
- cert_expires: Oct  3 05:09:34 2026 GMT
  host: lightsprint.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightsprint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightsprint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lightsprint
provider_slug: lightsprint
slug: lightsprint-domain-security
source_filename: lightsprint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lightsprint.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 05:09:34 2026 GMT\n  hsts: false\ndomains:\n- domain: lightsprint.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightsprint/refs/heads/main/security/lightsprint-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Developer Tools
- Artificial Intelligence
- Agents
- Software Development
- Project Management
- Code Generation
- Team Collaboration
---
