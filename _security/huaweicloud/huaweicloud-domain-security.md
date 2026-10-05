---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: huaweicloud.com
  spf: true
hosts:
- cert_expires: Mar 25 05:21:23 2027 GMT
  host: www.huaweicloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Huaweicloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Huawei Cloud, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Huawei Cloud
provider_slug: huaweicloud
slug: huaweicloud-domain-security
source_filename: huaweicloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.huaweicloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 25 05:21:23 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: huaweicloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/huaweicloud/refs/heads/main/security/huaweicloud-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Cloud
- Infrastructure-as-a-Service
- Platform-as-a-Service
- Artificial Intelligence
---
