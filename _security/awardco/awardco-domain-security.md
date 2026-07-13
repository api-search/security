---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: awardco.com
  spf: true
hosts:
- cert_expires: Oct  1 00:58:16 2026 GMT
  host: www.awardco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  6 06:02:13 2026 GMT
  host: code.awardco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug  6 06:02:13 2026 GMT
  host: api.awardco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Awardco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Awardco, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Awardco
provider_slug: awardco
slug: awardco-domain-security
source_filename: awardco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.awardco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 00:58:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: code.awardco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  6 06:02:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.awardco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  6 06:02:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: awardco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/awardco/refs/heads/main/security/awardco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Employee Recognition
- Rewards
- Engagement
- HR Tech
- Incentives
- Points
---
