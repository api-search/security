---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jdt.com.cn
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: jdcloud.com
  spf: false
hosts:
- cert_expires: Dec 19 05:50:13 2026 GMT
  host: www.jdt.com.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 02:05:24 2026 GMT
  host: docs.jdcloud.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 02:05:24 2026 GMT
  host: vm.jdcloud-api.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jd Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JD Technology, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: JD Technology
provider_slug: jd-technology
slug: jd-technology-domain-security
source_filename: jd-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jdt.com.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 05:50:13 2026 GMT\n  hsts: false\n- host: docs.jdcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 02:05:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: vm.jdcloud-api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 02:05:24 2026 GMT\n  hsts: null\ndomains:\n- domain: jdt.com.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: jdcloud.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jd-technology/refs/heads/main/security/jd-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Technology
- Cloud
- Cloud Computing
- Infrastructure
- Fintech
- Artificial Intelligence
- Developer Platform
- OpenAPI
- China
---
