---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: astrobotic.com
  spf: true
hosts:
- cert_expires: Sep 10 15:24:51 2026 GMT
  host: www.astrobotic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Astrobotic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Astrobotic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Astrobotic
provider_slug: astrobotic
slug: astrobotic-domain-security
source_filename: astrobotic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.astrobotic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 15:24:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: astrobotic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/astrobotic/refs/heads/main/security/astrobotic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Space
- Aerospace
- Robotics
- Lunar Logistics
- Spacecraft
- Satellites
- Defense and Space
---
