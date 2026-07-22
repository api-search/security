---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lemonbox.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: lemonbox.com.cn
  spf: false
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: www.lemonbox.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: www.lemonbox.com.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lemonbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LemonBox, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LemonBox
provider_slug: lemonbox
slug: lemonbox-domain-security
source_filename: lemonbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lemonbox.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: false\n- host: www.lemonbox.com.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lemonbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: lemonbox.com.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lemonbox/refs/heads/main/security/lemonbox-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Consumer
- Health
- Nutrition
- Supplements
- Personalization
- Artificial Intelligence
- Direct to Consumer
- E-Commerce
- China
---
