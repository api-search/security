---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: skechers.com
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: www.skechers.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skechers Usa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skechers U.S.A., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Skechers U.S.A.
provider_slug: skechers-usa
slug: skechers-usa-domain-security
source_filename: skechers-usa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.skechers.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: skechers.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skechers-usa/refs/heads/main/security/skechers-usa-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Footwear
- Retail
- E-Commerce
- Fortune 500
- Direct-to-Consumer
- Lifestyle
---
