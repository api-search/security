---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qq.com
  spf: true
hosts:
- cert_expires: Jan 28 06:39:19 2027 GMT
  host: y.qq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qq Music Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QQ Music, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: QQ Music
provider_slug: qq-music
slug: qq-music-domain-security
source_filename: qq-music-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: y.qq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 06:39:19 2027 GMT\n  hsts: false\ndomains:\n- domain: qq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qq-music/refs/heads/main/security/qq-music-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Music
- Streaming
- Tencent
- China
- Entertainment
---
