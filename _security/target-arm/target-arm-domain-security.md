---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: targetarm.com
  spf: true
hosts:
- cert_expires: Oct 18 03:23:21 2026 GMT
  host: targetarm.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Target Arm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Target Arm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Target Arm
provider_slug: target-arm
slug: target-arm-domain-security
source_filename: target-arm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: targetarm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 03:23:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: targetarm.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/target-arm/refs/heads/main/security/target-arm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Robotics
- Drones
- UAV
- Autonomous Systems
- Defense
- Hardware
- Aerospace
---
