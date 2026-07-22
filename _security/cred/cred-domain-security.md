---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cred.club
  spf: true
hosts:
- cert_expires: Jan 23 12:08:43 2027 GMT
  host: cred.club
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cred Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CRED, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CRED
provider_slug: cred
slug: cred-domain-security
source_filename: cred-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cred.club\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 12:08:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cred.club\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cred/refs/heads/main/security/cred-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Consumer Fintech
- Credit Cards
- Bill Payment
- Rewards
- UPI
- Lending
- India
---
