---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cureapp.co.jp
  spf: false
hosts:
- cert_expires: Apr 23 23:59:59 2027 GMT
  host: cureapp.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cureapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CureApp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CureApp
provider_slug: cureapp
slug: cureapp-domain-security
source_filename: cureapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cureapp.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 23 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: cureapp.co.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cureapp/refs/heads/main/security/cureapp-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- DigitalTherapeutics
- Healthcare
- Japan
- Software
---
