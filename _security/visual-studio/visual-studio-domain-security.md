---
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: npmjs.com
  spf: true
hosts:
- cert_expires: Mar  1 19:38:54 2027 GMT
  host: visualstudio.microsoft.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 03:32:50 2026 GMT
  host: www.npmjs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 13:38:08 2026 GMT
  host: marketplace.visualstudio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Visual Studio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Visual Studio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Visual Studio
provider_slug: visual-studio
slug: visual-studio-domain-security
source_filename: visual-studio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: visualstudio.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 19:38:54 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: www.npmjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 03:32:50 2026 GMT\n  hsts: null\n- host: marketplace.visualstudio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 13:38:08 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: npmjs.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visual-studio/refs/heads/main/security/visual-studio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- IDE
- Developer Tools
- Microsoft
- Code Collaboration
- Marketplace
- Extensions
---
