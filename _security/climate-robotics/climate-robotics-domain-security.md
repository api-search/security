---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: climaterobotics.network
  spf: true
hosts:
- cert_expires: Mar 29 08:36:11 2027 GMT
  host: climaterobotics.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Climate Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Climate Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Climate Robotics
provider_slug: climate-robotics
slug: climate-robotics-domain-security
source_filename: climate-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: climaterobotics.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 29 08:36:11 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: climaterobotics.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/climate-robotics/refs/heads/main/security/climate-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Climate
- Robotics
- Community
- Sustainability
- Open Source
---
