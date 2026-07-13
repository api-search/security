---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: talkwalker.com
  spf: true
hosts:
- cert_expires: Aug 22 11:37:02 2026 GMT
  host: www.talkwalker.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: developer.talkwalker.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: api.talkwalker.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Talkwalker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Talkwalker, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Talkwalker
provider_slug: talkwalker
slug: talkwalker-domain-security
source_filename: talkwalker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.talkwalker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 11:37:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.talkwalker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: false\n- host: api.talkwalker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: talkwalker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/talkwalker/refs/heads/main/security/talkwalker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Media Analytics
- Social Listening
- Brand Monitoring
- Sentiment Analysis
- Media Monitoring
- Campaign Analytics
---
