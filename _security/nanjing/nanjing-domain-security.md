---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nju.edu.cn
  spf: true
hosts:
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: www.nju.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: itsc.nju.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: authserver.nju.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nanjing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nanjing University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nanjing University
provider_slug: nanjing
slug: nanjing-domain-security
source_filename: nanjing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nju.edu.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: false\n- host: itsc.nju.edu.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: false\n- host: authserver.nju.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: nju.edu.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nanjing/refs/heads/main/security/nanjing-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Education
- Higher Education
- University
- Research
- China
- Authentication
---
