---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 700credit.com
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: 700credit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 700 Credit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 700 Credit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 700 Credit
provider_slug: 700credit
slug: 700credit-domain-security
source_filename: 700credit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 700credit.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 700credit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/700credit/security/700credit-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Credit
- Compliance
- Identity Verification
- Automotive
- Dealers
---
