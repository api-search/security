---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fixmypdfonline.com
  spf: false
hosts:
- cert_expires: Jan  3 00:09:49 2027 GMT
  host: fixmypdfonline.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FixMyPDF Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FixMyPDF, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: FixMyPDF
provider_slug: fixmypdfonline-com
slug: fixmypdfonline-com-domain-security
source_filename: fixmypdfonline-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fixmypdfonline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 00:09:49 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: fixmypdfonline.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fixmypdfonline-com/security/fixmypdfonline-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- PDF
- Editing
- Online Tool
- Free Tier
- Privacy
---
