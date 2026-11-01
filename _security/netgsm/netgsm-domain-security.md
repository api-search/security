---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: netgsm.com.tr
  spf: true
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: www.netgsm.com.tr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Netgsm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netgsm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Netgsm
provider_slug: netgsm
slug: netgsm-domain-security
source_filename: netgsm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.netgsm.com.tr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: netgsm.com.tr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/netgsm/security/netgsm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SMS
- VoIP
- Internet
- OTP
- IoT
---
