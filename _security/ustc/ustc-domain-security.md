---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ustc.edu.cn
  spf: true
hosts:
- cert_expires: Aug 17 23:59:59 2026 GMT
  host: en.ustc.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 08:05:39 2026 GMT
  host: mirrors.ustc.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 14:43:29 2026 GMT
  host: passport.ustc.edu.cn
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ustc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Science and Technology of China, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: University of Science and Technology of China
provider_slug: ustc
slug: ustc-domain-security
source_filename: ustc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.ustc.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 23:59:59 2026 GMT\n  hsts: false\n- host: mirrors.ustc.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 08:05:39 2026 GMT\n  hsts: false\n- host: passport.ustc.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 14:43:29 2026 GMT\n  hsts: null\ndomains:\n- domain: ustc.edu.cn\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ustc/refs/heads/main/security/ustc-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research
- China
- Open Source Mirror
---
