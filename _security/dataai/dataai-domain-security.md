---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: data.ai
  spf: true
hosts:
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: www.data.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dataai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Data.ai
provider_slug: dataai
slug: dataai-domain-security
source_filename: dataai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.data.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: data.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dataai/refs/heads/main/security/dataai-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Analytics
- Mobile
- App Store
- Market Data
- Business Intelligence
- App Analytics
---
