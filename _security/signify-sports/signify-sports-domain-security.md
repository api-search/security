---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: signify.ai
  spf: true
hosts:
- cert_expires: Oct  1 22:10:46 2026 GMT
  host: www.signify.ai
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Signify Sports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Signify Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Signify Group
provider_slug: signify-sports
slug: signify-sports-domain-security
source_filename: signify-sports-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.signify.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 22:10:46 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: signify.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signify-sports/refs/heads/main/security/signify-sports-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Sports
- Online Abuse
- Threat Intelligence
- Content Moderation
- Athlete Protection
- Trust And Safety
- OSINT
- Open Source Intelligence
- Social Media Monitoring
- Hate Speech Detection
- Augmented Intelligence
- Natural Language Understanding
- Brand Protection
- Risk Management
- Data Science
---
