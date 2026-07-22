---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: intuitionrobotics.com
  spf: true
hosts:
- cert_expires: Sep 11 06:45:34 2026 GMT
  host: www.intuitionrobotics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intuition Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Intuition Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Intuition Robotics
provider_slug: intuition-robotics
slug: intuition-robotics-domain-security
source_filename: intuition-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.intuitionrobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 06:45:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: intuitionrobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intuition-robotics/refs/heads/main/security/intuition-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Artificial Intelligence
- Eldercare
- Consumer Electronics
- Healthcare
- Agentic Commerce
---
