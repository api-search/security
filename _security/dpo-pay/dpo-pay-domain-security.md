---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dpogroup.com
  spf: true
hosts:
- cert_expires: Jan 10 15:42:50 2027 GMT
  host: dpogroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dpo Pay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DPO Pay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DPO Pay
provider_slug: dpo-pay
slug: dpo-pay-domain-security
source_filename: dpo-pay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dpogroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 15:42:50 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dpogroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dpo-pay/security/dpo-pay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Africa
- FinTech
- E‑commerce
---
