---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tju.edu.cn
  spf: true
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: en.tju.edu.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jul 21 23:59:59 2026 GMT
  host: opac.lib.tju.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tianjin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tianjin University, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Tianjin University
provider_slug: tianjin
slug: tianjin-domain-security
source_filename: tianjin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.tju.edu.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: opac.lib.tju.edu.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tju.edu.cn\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tianjin/refs/heads/main/security/tianjin-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- China
- Tianjin
---
