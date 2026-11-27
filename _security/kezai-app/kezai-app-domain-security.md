---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kezai.app
  spf: true
hosts:
- cert_expires: Jan  6 02:36:28 2027 GMT
  host: kezai.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kezai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kezai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kezai
provider_slug: kezai-app
slug: kezai-app-domain-security
source_filename: kezai-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kezai.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 02:36:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kezai.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kezai-app/security/kezai-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- PersonalJournal
- Media Tracking
- PrivacyFocused
- Free Tier
---
