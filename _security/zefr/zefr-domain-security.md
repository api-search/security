---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: zefr.com
  spf: true
hosts:
- cert_expires: Oct 19 07:24:55 2026 GMT
  host: zefr.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zefr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zefr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Zefr
provider_slug: zefr
slug: zefr-domain-security
source_filename: zefr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zefr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 07:24:55 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: zefr.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zefr/refs/heads/main/security/zefr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Adtech
- Brand Safety
- Brand Suitability
- Content Intelligence
- Video
- Social Media
- Advertising
---
