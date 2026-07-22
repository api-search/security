---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fernride.com
  spf: true
hosts:
- cert_expires: Oct  3 03:41:31 2026 GMT
  host: www.fernride.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fernride Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fernride, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fernride
provider_slug: fernride
slug: fernride-domain-security
source_filename: fernride-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fernride.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:41:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fernride.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fernride/refs/heads/main/security/fernride-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Autonomous Vehicles
- Trucking
- Automation
- Fleet Management
- Supply Chain
- Teleoperation
---
