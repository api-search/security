---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 163.com
  spf: true
hosts:
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: music.163.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Netease Cloud Music Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NetEase Cloud Music, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NetEase Cloud Music
provider_slug: netease-cloud-music
slug: netease-cloud-music-domain-security
source_filename: netease-cloud-music-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: music.163.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: 163.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/netease-cloud-music/refs/heads/main/security/netease-cloud-music-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Music
- Streaming
- Chinese
- API
---
