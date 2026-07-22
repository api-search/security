---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bearflagrobotics.com
  spf: true
hosts:
- cert_expires: Sep  3 07:46:52 2026 GMT
  host: bearflagrobotics.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bear Flag Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bear Flag Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bear Flag Robotics
provider_slug: bear-flag-robotics
slug: bear-flag-robotics-domain-security
source_filename: bear-flag-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bearflagrobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 07:46:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: bearflagrobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bear-flag-robotics/refs/heads/main/security/bear-flag-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hardware
- Robotics
- Autonomous Vehicles
- Agriculture
- Agtech
---
