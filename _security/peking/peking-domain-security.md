---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pku.edu.cn
  spf: true
hosts:
- cert_expires: Mar 24 05:59:59 2027 GMT
  host: english.pku.edu.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 24 05:59:59 2027 GMT
  host: opendata.pku.edu.cn
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Peking Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peking University, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Peking University
provider_slug: peking
slug: peking-domain-security
source_filename: peking-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: english.pku.edu.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 24 05:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: opendata.pku.edu.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 24 05:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: pku.edu.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peking/refs/heads/main/security/peking-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- China
---
