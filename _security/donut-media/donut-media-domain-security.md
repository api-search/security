---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: donut.media
  spf: true
hosts:
- cert_expires: Aug 23 22:21:01 2026 GMT
  host: donut.media
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Donut Media Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Donut Media, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Donut Media
provider_slug: donut-media
slug: donut-media-domain-security
source_filename: donut-media-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: donut.media\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 22:21:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: donut.media\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/donut-media/refs/heads/main/security/donut-media-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- Automotive
- Entertainment
- Video
- YouTube
- Ecommerce
- Merchandise
- Podcast
---
