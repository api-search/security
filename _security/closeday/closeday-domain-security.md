---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: closeday.com
  spf: true
hosts:
- cert_expires: Jan  7 21:23:15 2027 GMT
  host: www.closeday.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Closeday Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloseDay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CloseDay
provider_slug: closeday
slug: closeday-domain-security
source_filename: closeday-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.closeday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 21:23:15 2027 GMT\n  hsts: false\ndomains:\n- domain: closeday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/closeday/security/closeday-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company Closure
- Insolvency Services
- Business Liquidation
- UK Compliance
- Asset Realisation
---
