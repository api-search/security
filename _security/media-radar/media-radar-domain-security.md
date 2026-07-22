---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mediaradar.com
  spf: true
hosts:
- cert_expires: Sep 19 01:38:27 2026 GMT
  host: mediaradar.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Media Radar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Media Radar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Media Radar
provider_slug: media-radar
slug: media-radar-domain-security
source_filename: media-radar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mediaradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 01:38:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mediaradar.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/media-radar/refs/heads/main/security/media-radar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Commerce
- Advertising Intelligence
- Marketing Intelligence
- Competitive Intelligence
- Advertising
- Media
- Data
---
