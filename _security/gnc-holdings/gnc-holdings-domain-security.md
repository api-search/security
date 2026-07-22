---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gnc.com
  spf: true
hosts:
- cert_expires: Sep 23 17:49:25 2026 GMT
  host: www.gnc.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gnc Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GNC Holdings, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GNC Holdings
provider_slug: gnc-holdings
slug: gnc-holdings-domain-security
source_filename: gnc-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gnc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 17:49:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: gnc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gnc-holdings/refs/heads/main/security/gnc-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Diet
- Health
- Nutrition
- Retail
- Sports Nutrition
- Supplements
- Vitamins
- Wellness
- Fortune 1000
---
