---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: yubhub.co
  spf: true
hosts:
- cert_expires: Jan 25 01:15:06 2027 GMT
  host: yubhub.co
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yubhub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YubHub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: YubHub
provider_slug: yubhub
slug: yubhub-domain-security
source_filename: yubhub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yubhub.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 01:15:06 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: yubhub.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/yubhub/security/yubhub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- JobFeed
- Recruitment
- API
- UK
- DataEnrichment
---
