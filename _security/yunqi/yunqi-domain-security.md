---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yunqi.tech
  spf: true
hosts:
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: www.yunqi.tech
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yunqi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yunqi (ClickZetta / Singdata Lakehouse), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Yunqi (ClickZetta / Singdata Lakehouse)
provider_slug: yunqi
slug: yunqi-domain-security
source_filename: yunqi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yunqi.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: yunqi.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yunqi/refs/heads/main/security/yunqi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data
- Lakehouse
- Analytics
- SQL
- Cloud
- Data Engineering
- AI
- Apache Iceberg
- Database
---
