---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: reliable.co
  spf: true
hosts:
- cert_expires: Aug 14 18:11:05 2026 GMT
  host: reliable.co
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reliable Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reliable Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Reliable Robotics
provider_slug: reliable-robotics
slug: reliable-robotics-domain-security
source_filename: reliable-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reliable.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 18:11:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: reliable.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reliable-robotics/refs/heads/main/security/reliable-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Aerospace
- Automation
- Autonomy
- Cargo Aviation
- Defense
- FAA Certification
- General Aviation
- Remote Piloting
- Uncrewed Aircraft
---
