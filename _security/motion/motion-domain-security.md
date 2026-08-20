---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: motionapp.com
  spf: true
hosts:
- cert_expires: Oct 14 16:08:28 2026 GMT
  host: motionapp.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 01:19:33 2026 GMT
  host: projects.motionapp.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Motion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motion, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Motion
provider_slug: motion
slug: motion-domain-security
source_filename: motion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: motionapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 16:08:28 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: projects.motionapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 01:19:33 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: motionapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motion/refs/heads/main/security/motion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Creative Analytics
- Advertising
- Marketing Analytics
- Performance Marketing
- Ad Reporting
- Creative Strategy
- Software-as-a-Service
- MCP
- Agent Surface
---
