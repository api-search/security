---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 1yongcloud.com
  spf: false
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: www.1yongcloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Yongcloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1yongcloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: 1yongcloud
provider_slug: 1yongcloud
slug: 1yongcloud-domain-security
source_filename: 1yongcloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.1yongcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 1yongcloud.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1yongcloud/refs/heads/main/security/1yongcloud-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Oncology
- Artificial Intelligence
- Big Data
- Medical Data
- China
- Hospital
---
