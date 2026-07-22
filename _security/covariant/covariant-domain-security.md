---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: covariant.ai
  spf: true
hosts:
- cert_expires: Aug 18 19:53:51 2026 GMT
  host: covariant.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Covariant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Covariant, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Covariant
provider_slug: covariant
slug: covariant-domain-security
source_filename: covariant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: covariant.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 19:53:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: covariant.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/covariant/refs/heads/main/security/covariant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Warehouse Robotics
- Warehouse Automation
- Industrial Robotics
- AI Robotics
- Embodied AI
- Foundation Models
- Robotics Foundation Model
- RFM-1
- Covariant Brain
- Picking Robots
- Depalletization
- Sortation
- Goods-to-Person
- Logistics
- Supply Chain
- Manufacturing
---
