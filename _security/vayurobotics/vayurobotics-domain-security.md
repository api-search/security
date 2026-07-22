---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vayurobotics.com
  spf: true
hosts:
- cert_expires: Sep 25 18:12:42 2026 GMT
  host: www.vayurobotics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vayurobotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vayu Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vayu Robotics
provider_slug: vayurobotics
slug: vayurobotics-domain-security
source_filename: vayurobotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vayurobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 18:12:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vayurobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vayurobotics/refs/heads/main/security/vayurobotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Autonomous Vehicles
- Artificial Intelligence
- Sensors
- Delivery
- Foundation Models
---
