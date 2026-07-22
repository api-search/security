---
description: ''
domains:
- caa:
  - 48ccba35a7cb43bdaf98e095f720d263.vip1.huaweicloudwaf.com.
  dmarc: false
  dnssec: true
  domain: guokang.com
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: guokang.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Guokang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for guokang, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: guokang
provider_slug: guokang
slug: guokang-domain-security
source_filename: guokang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: guokang.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: guokang.com\n  dnssec: true\n  caa:\n  - 48ccba35a7cb43bdaf98e095f720d263.vip1.huaweicloudwaf.com.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guokang/refs/heads/main/security/guokang-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Health
- Healthcare
- Health Management
- Corporate Wellness
- Private Doctor
- China
---
