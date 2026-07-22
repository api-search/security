---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: therecount.com
  spf: true
hosts:
- cert_expires: Sep 21 08:50:48 2026 GMT
  host: therecount.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Recount Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Recount Media, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Recount Media
provider_slug: recount-media
slug: recount-media-domain-security
source_filename: recount-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: therecount.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:50:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: therecount.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recount-media/refs/heads/main/security/recount-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- News
- Politics
- Journalism
- Video
- Newsletter
---
