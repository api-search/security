---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: iclip.cn
  spf: false
hosts:
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: iclip.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: iClip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iClip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: iClip
provider_slug: iclip-cn
slug: iclip-cn-domain-security
source_filename: iclip-cn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iclip.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: iclip.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/iclip-cn/security/iclip-cn-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
