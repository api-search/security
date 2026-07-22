---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: airquality.com.cn
  spf: true
hosts:
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: airquality.com.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Airquality Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for airquality, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: airquality
provider_slug: airquality
slug: airquality-domain-security
source_filename: airquality-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airquality.com.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: airquality.com.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airquality/refs/heads/main/security/airquality-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Air Quality
- Air Purification
- Environmental
- Manufacturing
- Hardware
- IoT
- China
---
