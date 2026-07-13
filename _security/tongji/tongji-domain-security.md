---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tongji.edu.cn
  spf: true
hosts:
- cert_expires: Oct 31 11:59:59 2026 GMT
  host: www.tongji.edu.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 11:59:59 2026 GMT
  host: en.tongji.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 11:59:59 2026 GMT
  host: api.tongji.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tongji Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tongji University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tongji University
provider_slug: tongji
slug: tongji-domain-security
source_filename: tongji-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tongji.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 11:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: en.tongji.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 11:59:59 2026 GMT\n  hsts: false\n- host: api.tongji.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 11:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tongji.edu.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tongji/refs/heads/main/security/tongji-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- China
- Shanghai
- Open Platform
- Campus Data
---
