---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wellxai.com
  spf: true
hosts:
- cert_expires: Sep 13 18:28:40 2026 GMT
  host: wellxai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wellxai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wellxai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wellxai
provider_slug: wellxai
slug: wellxai-domain-security
source_filename: wellxai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wellxai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:28:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wellxai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wellxai/refs/heads/main/security/wellxai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Insurance
- Insurtech
- Digital Health
- Wellness
- Behavior Change
- Rewards
- Wearables
- Mobile
- UAE
---
