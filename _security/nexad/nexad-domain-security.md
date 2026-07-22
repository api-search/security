---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nex.ad
  spf: true
hosts:
- cert_expires: Sep  5 11:09:05 2026 GMT
  host: nex.ad
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nexad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nexad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nexad
provider_slug: nexad
slug: nexad-domain-security
source_filename: nexad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nex.ad\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 11:09:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nex.ad\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexad/refs/heads/main/security/nexad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Advertising
- Marketing
- Marketing Automation
- Contextual Advertising
- Mobile SDK
- Agent
---
