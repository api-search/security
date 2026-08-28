---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: yazio.com
  spf: true
hosts:
- cert_expires: Nov 12 06:51:11 2026 GMT
  host: www.yazio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yazio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YAZIO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: YAZIO
provider_slug: yazio
slug: yazio-domain-security
source_filename: yazio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yazio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 06:51:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yazio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yazio/refs/heads/main/security/yazio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Digital Health
- Nutrition
- Calorie Tracking
- Weight Management
- Intermittent Fasting
- Fitness
- Consumer Health
- Mobile Applications
- Germany
---
