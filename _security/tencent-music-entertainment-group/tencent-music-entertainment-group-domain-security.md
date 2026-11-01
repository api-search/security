---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tencentmusic.com
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.tencentmusic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tencent Music Entertainment Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tencent Music Entertainment Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tencent Music Entertainment Group
provider_slug: tencent-music-entertainment-group
slug: tencent-music-entertainment-group-domain-security
source_filename: tencent-music-entertainment-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tencentmusic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tencentmusic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/tencent-music-entertainment-group/security/tencent-music-entertainment-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Music
- Streaming
- Entertainment
- China
---
