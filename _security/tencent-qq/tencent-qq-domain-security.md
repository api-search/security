---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qq.com
  spf: true
hosts:
- cert_expires: Jan 21 02:31:34 2027 GMT
  host: connect.qq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tencent Qq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tencent QQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tencent QQ
provider_slug: tencent-qq
slug: tencent-qq-domain-security
source_filename: tencent-qq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: connect.qq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 02:31:34 2027 GMT\n  hsts: false\ndomains:\n- domain: qq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/tencent-qq/security/tencent-qq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
