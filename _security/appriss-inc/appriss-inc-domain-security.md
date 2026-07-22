---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apprissretail.com
  spf: true
hosts:
- cert_expires: Oct  4 21:29:36 2026 GMT
  host: apprissretail.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appriss Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Appriss Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Appriss Inc.
provider_slug: appriss-inc
slug: appriss-inc-domain-security
source_filename: appriss-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apprissretail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:29:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apprissretail.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appriss-inc/refs/heads/main/security/appriss-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Loss Prevention
- Returns Management
- Fraud Prevention
- Analytics
- Retail Technology
---
