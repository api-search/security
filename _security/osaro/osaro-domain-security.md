---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: osaro.com
  spf: true
hosts:
- cert_expires: Sep 27 00:32:36 2026 GMT
  host: www.osaro.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Osaro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OSARO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OSARO
provider_slug: osaro
slug: osaro-domain-security
source_filename: osaro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.osaro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 00:32:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: osaro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osaro/refs/heads/main/security/osaro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Artificial Intelligence
- Machine Learning
- Warehouse Automation
- Logistics
- Supply Chain
- Computer Vision
- Manufacturing
---
