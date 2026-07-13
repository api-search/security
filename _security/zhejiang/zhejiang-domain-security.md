---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: zju.edu.cn
  spf: true
hosts:
- cert_expires: Mar 27 06:59:59 2027 GMT
  host: www.zju.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 27 06:59:59 2027 GMT
  host: zjuam.zju.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar 27 06:59:59 2027 GMT
  host: idp.zju.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zhejiang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zhejiang University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Zhejiang University
provider_slug: zhejiang
slug: zhejiang-domain-security
source_filename: zhejiang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zju.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 06:59:59 2027 GMT\n  hsts: false\n- host: zjuam.zju.edu.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 27 06:59:59 2027 GMT\n  hsts: false\n- host: idp.zju.edu.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 27 06:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: zju.edu.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zhejiang/refs/heads/main/security/zhejiang-domain-security.yml
summary_line: TLSv1.3
tags:
- Education
- Higher Education
- University
- Research
- China
- Identity
- SSO
---
