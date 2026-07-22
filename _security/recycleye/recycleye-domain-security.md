---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: recycleye.com
  spf: true
hosts:
- cert_expires: Sep 29 20:14:43 2026 GMT
  host: recycleye.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Recycleye Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recycleye, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Recycleye
provider_slug: recycleye
slug: recycleye-domain-security
source_filename: recycleye-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: recycleye.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:14:43 2026 GMT\n  hsts: false\ndomains:\n- domain: recycleye.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recycleye/refs/heads/main/security/recycleye-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Recycling
- Waste Management
- Artificial Intelligence
- Computer Vision
- Robotics
- Sustainability
- Circular Economy
---
