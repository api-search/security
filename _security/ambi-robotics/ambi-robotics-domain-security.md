---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ambirobotics.com
  spf: true
hosts:
- cert_expires: Aug 21 03:27:54 2026 GMT
  host: www.ambirobotics.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ambi Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ambi Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ambi Robotics
provider_slug: ambi-robotics
slug: ambi-robotics-domain-security
source_filename: ambi-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ambirobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 03:27:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ambirobotics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambi-robotics/refs/heads/main/security/ambi-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Robotics
- AI Robotics
- Embodied AI
- Parcel Sortation
- Parcel Induction
- Logistics
- Last Mile
- Middle Mile
- Reverse Logistics
- Warehouse Automation
- Ecommerce Fulfillment
- Postal Automation
- Foundation Models
- Sim2Real
- Computer Vision
- Fleet Management
- AmbiOS
- AmbiSort
- AmbiStack
- AmbiVision
- PRIME-1
- Pitney Bowes
- Berkeley
- Hardware
---
