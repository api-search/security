---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: plusonerobotics.com
  spf: true
hosts:
- cert_expires: Sep 11 19:13:46 2026 GMT
  host: www.plusonerobotics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plus One Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plus One Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Plus One Robotics
provider_slug: plus-one-robotics
slug: plus-one-robotics-domain-security
source_filename: plus-one-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plusonerobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 19:13:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: plusonerobotics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plus-one-robotics/refs/heads/main/security/plus-one-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Robotics
- Warehouse Automation
- Computer-Vision
- Artificial Intelligence
- Logistics
- Supply Chain
- Parcel
- Depalletizing
- Palletizing
---
