---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: shardsecure.com
  spf: true
hosts:
- cert_expires: Aug 21 14:54:29 2026 GMT
  host: shardsecure.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shardsecure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShardSecure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ShardSecure
provider_slug: shardsecure
slug: shardsecure-domain-security
source_filename: shardsecure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shardsecure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 14:54:29 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\ndomains:\n- domain: shardsecure.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shardsecure/refs/heads/main/security/shardsecure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Security
- Encryption
- Ransomware Protection
- Data Resilience
- Cloud Security
- Data Privacy
- AI Security
---
