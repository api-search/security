---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fudan.edu.cn
  spf: true
hosts:
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: www.fudan.edu.cn
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr 10 23:59:59 2027 GMT
  host: dvn.fudan.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fudan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fudan University, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fudan University
provider_slug: fudan
slug: fudan-domain-security
source_filename: fudan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fudan.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: null\n- host: dvn.fudan.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: fudan.edu.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fudan/refs/heads/main/security/fudan-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- China
- Shanghai
---
