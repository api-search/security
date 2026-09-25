---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agrist.com
  spf: true
hosts:
- cert_expires: Oct 26 00:00:01 2026 GMT
  host: agrist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agrist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agrist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Agrist
provider_slug: agrist
slug: agrist-domain-security
source_filename: agrist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agrist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 00:00:01 2026 GMT\n  hsts: false\ndomains:\n- domain: agrist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agrist/refs/heads/main/security/agrist-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Agriculture
- AgTech
- Robotics
- Artificial Intelligence
- Computer Vision
- Smart Farming
- Greenhouse
- Automation
- Food Tech
- Deep Tech
- Japan
---
