---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: realitydefender.com
  spf: true
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 128 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: false
  dnssec: false
  domain: realitydefender.xyz
  spf: false
hosts:
- cert_expires: Sep 27 06:34:39 2026 GMT
  host: www.realitydefender.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 13:40:11 2026 GMT
  host: docs.realitydefender.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 00:43:11 2026 GMT
  host: api.prd.realitydefender.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reality Defender Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reality Defender, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Reality Defender
provider_slug: reality-defender
slug: reality-defender-domain-security
source_filename: reality-defender-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.realitydefender.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 06:34:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.realitydefender.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:40:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.prd.realitydefender.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 00:43:11 2026 GMT\n  hsts: null\ndomains:\n- domain: realitydefender.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: realitydefender.xyz\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 128 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reality-defender/refs/heads/main/security/reality-defender-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Deepfake Detection
- Artificial Intelligence
- Media Authentication
- Content Moderation
- Security
- Fraud Prevention
- Synthetic Media
- Machine Learning
---
