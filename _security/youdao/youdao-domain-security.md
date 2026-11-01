---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: youdao.com
  spf: true
hosts:
- cert_expires: May  8 23:59:59 2027 GMT
  host: youdao.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Youdao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NetEase Youdao, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NetEase Youdao
provider_slug: youdao
slug: youdao-domain-security
source_filename: youdao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: youdao.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: youdao.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/youdao/security/youdao-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Education
- Language
- AI
- Cloud
- Enterprise
---
