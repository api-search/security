---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: nimble.ai
  spf: true
hosts:
- cert_expires: Sep 28 23:12:57 2026 GMT
  host: nimble.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nimble Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nimble Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Nimble Robotics
provider_slug: nimble-robotics
slug: nimble-robotics-domain-security
source_filename: nimble-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nimble.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:12:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nimble.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nimble-robotics/refs/heads/main/security/nimble-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Robotics
- Logistics
- Fulfillment
- Ecommerce
- Automation
- 3PL
- Supply Chain
---
