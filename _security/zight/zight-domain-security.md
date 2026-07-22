---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: zight.com
  spf: true
hosts:
- cert_expires: Sep  9 03:17:14 2026 GMT
  host: zight.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Zight
provider_slug: zight
slug: zight-domain-security
source_filename: zight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 03:17:14 2026 GMT\n  hsts: null\ndomains:\n- domain: zight.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zight/refs/heads/main/security/zight-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Screen Recording
- Screenshots
- Screen Capture
- Video Messaging
- Async Collaboration
- Visual Communication
- Productivity
- Annotation
- GIF
---
