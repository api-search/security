---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yuanfudao.com
  spf: true
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: www.yuanfudao.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yuanfudao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yuanfudao, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yuanfudao
provider_slug: yuanfudao
slug: yuanfudao-domain-security
source_filename: yuanfudao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yuanfudao.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: yuanfudao.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yuanfudao/refs/heads/main/security/yuanfudao-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Education
- EdTech
- Online Learning
- Tutoring
- Artificial Intelligence
- Mobile Applications
- China
---
