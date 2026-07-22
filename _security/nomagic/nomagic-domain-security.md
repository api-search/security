---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nomagic.ai
  spf: true
hosts:
- cert_expires: Oct 13 20:13:19 2026 GMT
  host: nomagic.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nomagic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nomagic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nomagic
provider_slug: nomagic
slug: nomagic-domain-security
source_filename: nomagic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nomagic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 20:13:19 2026 GMT\n  hsts: false\ndomains:\n- domain: nomagic.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nomagic/refs/heads/main/security/nomagic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Robotics
- Warehouse Automation
- Physical AI
- Computer Vision
- Logistics
- Fulfillment
- Artificial Intelligence
---
