---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oneassist.in
  spf: true
hosts:
- cert_expires: Jan 28 10:01:36 2027 GMT
  host: www.oneassist.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: One Assist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for One Assist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: One Assist
provider_slug: one-assist
slug: one-assist-domain-security
source_filename: one-assist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oneassist.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 10:01:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: oneassist.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/one-assist/refs/heads/main/security/one-assist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- InsurTech
- Consumer Protection
- Extended Warranty
- Device Protection
- Fintech
- India
---
