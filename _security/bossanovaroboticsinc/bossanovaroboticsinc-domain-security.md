---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bossanova.com
  spf: true
hosts:
- cert_expires: Nov 28 11:14:20 2026 GMT
  host: www.bossanova.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bossanovaroboticsinc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bossanovaroboticsinc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bossanovaroboticsinc
provider_slug: bossanovaroboticsinc
slug: bossanovaroboticsinc-domain-security
source_filename: bossanovaroboticsinc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bossanova.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 11:14:20 2026 GMT\n  hsts: false\ndomains:\n- domain: bossanova.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bossanovaroboticsinc/refs/heads/main/security/bossanovaroboticsinc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Robotics
- Artificial Intelligence
- Retail Automation
- Inventory
- Startups
---
