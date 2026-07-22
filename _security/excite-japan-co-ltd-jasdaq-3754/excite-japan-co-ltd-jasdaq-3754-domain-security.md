---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: excite.co.jp
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.excite.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Excite Japan Co Ltd Jasdaq 3754 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Excite Japan Co., Ltd. (JASDAQ:3754), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Excite Japan Co., Ltd. (JASDAQ:3754)
provider_slug: excite-japan-co-ltd-jasdaq-3754
slug: excite-japan-co-ltd-jasdaq-3754-domain-security
source_filename: excite-japan-co-ltd-jasdaq-3754-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.excite.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: excite.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/excite-japan-co-ltd-jasdaq-3754/refs/heads/main/security/excite-japan-co-ltd-jasdaq-3754-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Japan
- Internet Media
- Web Portal
- Search
- Blogging
- Broadband
- ISP
- Translation
- SaaS
---
