---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: huaun.com
  spf: true
hosts:
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: www.huaun.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Huaun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Huaun, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Huaun
provider_slug: huaun
slug: huaun-domain-security
source_filename: huaun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.huaun.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: huaun.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huaun/refs/heads/main/security/huaun-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Enterprise
- Cybersecurity
- Attack Surface Management
- Vulnerability Management
- Threat Intelligence
- Penetration Testing
- Security
---
