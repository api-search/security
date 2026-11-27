---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: syln.cn
  spf: true
hosts:
- cert_expires: Feb  4 16:43:44 2027 GMT
  host: syln.cn
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: syln-cn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for syln-cn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: syln-cn
provider_slug: syln-cn
slug: syln-cn-domain-security
source_filename: syln-cn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: syln.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 16:43:44 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: syln.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/syln-cn/security/syln-cn-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
