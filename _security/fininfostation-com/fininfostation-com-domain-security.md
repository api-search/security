---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fininfostation.com
  spf: false
hosts:
- cert_expires: Jan  5 07:10:36 2027 GMT
  host: fininfostation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fininfostation Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 金融情報站, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: 金融情報站
provider_slug: fininfostation-com
slug: fininfostation-com-domain-security
source_filename: fininfostation-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fininfostation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 07:10:36 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fininfostation.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fininfostation-com/security/fininfostation-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Finance
- Data
- Taiwan
- ETFs
- Stocks
---
