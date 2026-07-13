---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: waifu.pics
  spf: true
hosts:
- cert_expires: Sep  7 10:59:34 2026 GMT
  host: waifu.pics
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Waifu Pics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Waifu.pics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Waifu.pics
provider_slug: waifu-pics
slug: waifu-pics-domain-security
source_filename: waifu-pics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: waifu.pics\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 10:59:34 2026 GMT\n  hsts: false\ndomains:\n- domain: waifu.pics\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waifu-pics/refs/heads/main/security/waifu-pics-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Anime
- Public APIs
---
