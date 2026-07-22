---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tutorabc.com
  spf: true
  spf_record: v=spf1 mx mx:spam.tutorabc.com ip4:60.251.28.84 ip4:60.251.28.85 ip4:210.242.31.58 ip4:61.219.187.0/24 ip4:211.72.13.0/24 ip4:60.251.53.0/24 ip4:60.251.28.0/24 ip4:152.101.54.122 -all
hosts:
- cert_valid: true
  host: www.tutorabc.com
  hsts: true
  hsts_max_age: 157670188
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tutorabc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TutorABC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TutorABC
provider_slug: tutorabc
slug: tutorabc-domain-security
source_filename: tutorabc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: dig + TLS/HTTP HEAD probe of tutorabc.com hosts\nhosts:\n  - host: www.tutorabc.com\n    https: true\n    tls_version: TLSv1.3\n    cert_valid: true\n    hsts: true\n    hsts_max_age: 157670188\ndomains:\n  - domain: tutorabc.com\n    dnssec: false\n    caa: []\n    spf: true\n    spf_record: \"v=spf1 mx mx:spam.tutorabc.com ip4:60.251.28.84 ip4:60.251.28.85 ip4:210.242.31.58 ip4:61.219.187.0/24 ip4:211.72.13.0/24 ip4:60.251.53.0/24 ip4:60.251.28.0/24 ip4:152.101.54.122 -all\"\n    dmarc: true\n    dmarc_policy: none\nnotes: >-\n  The apis.yml Website host tutorabc.com.cn does not resolve; the live consumer\n  platform is served from www.tutorabc.com (redirects to /site/zh-tw). Probe run\n  against the resolving production host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tutorabc/refs/heads/main/security/tutorabc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Online Learning
- Language Learning
- EdTech
- E-Learning
- Consumer
---
