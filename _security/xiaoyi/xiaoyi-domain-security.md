---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: xiaoyi.com
  spf: true
hosts:
- cert_expires: Aug 19 08:06:22 2026 GMT
  host: www.xiaoyi.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Xiaoyi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for xiaoyi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: xiaoyi
provider_slug: xiaoyi
slug: xiaoyi-domain-security
source_filename: xiaoyi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.xiaoyi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 19 08:06:22 2026 GMT\n  hsts: false\ndomains:\n- domain: xiaoyi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xiaoyi/refs/heads/main/security/xiaoyi-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Computer Vision
- Edge Computing
- Cameras
- Smart Home
- Consumer Electronics
- Internet of Things
- China
---
