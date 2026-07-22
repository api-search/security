---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xiaohongshu.com
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: xiaohongshu.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rednote Xiaohongshu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RedNote (Xiaohongshu), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RedNote (Xiaohongshu)
provider_slug: rednote-xiaohongshu
slug: rednote-xiaohongshu-domain-security
source_filename: rednote-xiaohongshu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xiaohongshu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: xiaohongshu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rednote-xiaohongshu/refs/heads/main/security/rednote-xiaohongshu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technology
- Social Media
- E-Commerce
- Content
- China
- Open Platform
---
