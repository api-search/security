---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anyware-robotics.com
  spf: true
hosts:
- cert_expires: Nov  8 05:55:33 2026 GMT
  host: anyware-robotics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anyware Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anyware Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Anyware Robotics
provider_slug: anyware-robotics
slug: anyware-robotics-domain-security
source_filename: anyware-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anyware-robotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 05:55:33 2026 GMT\n  hsts: false\ndomains:\n- domain: anyware-robotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anyware-robotics/refs/heads/main/security/anyware-robotics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Robotics
- AI
- Industrial Automation
- Deployable Robots
- Manufacturing
---
