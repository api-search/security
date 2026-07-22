---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getzoog.com
  spf: true
hosts:
- cert_expires: Aug 29 23:18:48 2026 GMT
  host: getzoog.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zoog Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zoog, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zoog
provider_slug: zoog
slug: zoog-domain-security
source_filename: zoog-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getzoog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:18:48 2026 GMT\n  hsts: false\ndomains:\n- domain: getzoog.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoog/refs/heads/main/security/zoog-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Children
- Education
- Family
- Video
- Storytelling
- Mobile App
- Entertainment
---
