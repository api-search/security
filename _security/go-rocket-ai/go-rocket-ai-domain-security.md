---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: go-rocket.ai
  spf: true
hosts:
- cert_expires: Jan  3 12:04:12 2027 GMT
  host: go-rocket.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Go Rocket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Go Rocket, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Go Rocket
provider_slug: go-rocket-ai
slug: go-rocket-ai-domain-security
source_filename: go-rocket-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: go-rocket.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 12:04:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: go-rocket.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/go-rocket-ai/security/go-rocket-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Video Ads
- Marketing
- UGC
- Multilingual
---
