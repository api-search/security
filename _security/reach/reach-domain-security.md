---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: reachpower.com
  spf: true
hosts:
- cert_expires: Oct  3 21:24:17 2026 GMT
  host: reachpower.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reach Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reach, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Reach
provider_slug: reach
slug: reach-domain-security
source_filename: reach-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reachpower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 21:24:17 2026 GMT\n  hsts: false\ndomains:\n- domain: reachpower.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reach/refs/heads/main/security/reach-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Wireless Power
- Energy
- Hardware
- Defense
- Robotics
- Climate
- IoT
---
