---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: treex.ai
  spf: true
hosts:
- cert_expires: Sep 15 12:37:24 2026 GMT
  host: treex.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Treex Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TreeX Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TreeX Robotics
provider_slug: treex-robotics
slug: treex-robotics-domain-security
source_filename: treex-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: treex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 12:37:24 2026 GMT\n  hsts: false\ndomains:\n- domain: treex.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/treex-robotics/refs/heads/main/security/treex-robotics-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Robotics
- Physical AI
- Autonomous Systems
- Field Operations
- Agriculture Technology
---
