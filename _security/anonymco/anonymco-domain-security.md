---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anonymco.com
  spf: true
hosts:
- cert_expires: Aug 19 14:22:01 2026 GMT
  host: anonymco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anonymco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anonym, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anonym
provider_slug: anonymco
slug: anonymco-domain-security
source_filename: anonymco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anonymco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 14:22:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anonymco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anonymco/refs/heads/main/security/anonymco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Advertising Technology
- Privacy
- Ad Measurement
- Confidential Computing
- Mozilla
---
