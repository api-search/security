---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: universal-robots.com
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.universal-robots.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:51:19 2026 GMT
  host: docs.universal-robots.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Universal Robots Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Universal Robots, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Universal Robots
provider_slug: universal-robots
slug: universal-robots-domain-security
source_filename: universal-robots-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.universal-robots.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: false\n- host: docs.universal-robots.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:51:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: universal-robots.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/universal-robots/refs/heads/main/security/universal-robots-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Robotics
- Collaborative Robots
- Cobots
- Industrial Automation
- Manufacturing
- PolyScope
- PolyScopeX
- URCaps
- URScript
- RTDE
- ROS
- ROS 2
- Teradyne
- Danish
- Hardware
---
