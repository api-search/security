---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agtonomy.com
  spf: true
hosts:
- cert_expires: Aug 19 01:28:53 2026 GMT
  host: agtonomy.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agtonomy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agtonomy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agtonomy
provider_slug: agtonomy
slug: agtonomy-domain-security
source_filename: agtonomy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agtonomy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 01:28:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agtonomy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agtonomy/refs/heads/main/security/agtonomy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Frontier Tech
- Agriculture
- AgTech
- Autonomy
- Physical AI
- Robotics
- Automation
---
