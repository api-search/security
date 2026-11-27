---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cashbackpro.org
  spf: true
hosts:
- cert_expires: Dec 14 01:57:04 2026 GMT
  host: cashbackpro.org
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CashbackPro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CashbackPro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CashbackPro
provider_slug: cashbackpro-org
slug: cashbackpro-org-domain-security
source_filename: cashbackpro-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cashbackpro.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 01:57:04 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: cashbackpro.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cashbackpro-org/security/cashbackpro-org-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cashback
- Affiliates
- AliExpress
- Rewards
- E-Commerce
---
