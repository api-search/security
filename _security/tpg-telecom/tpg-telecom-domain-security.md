---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tpgtelecom.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiary.io
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: www.tpgtelecom.com.au
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: contactsapiv1tgp.docs.apiary.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: api.messaging.tpgtelecom.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tpg Telecom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TPG Telecom, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TPG Telecom
provider_slug: tpg-telecom
slug: tpg-telecom-domain-security
source_filename: tpg-telecom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tpgtelecom.com.au\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: false\n- host: contactsapiv1tgp.docs.apiary.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: false\n- host: api.messaging.tpgtelecom.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: tpgtelecom.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: apiary.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tpg-telecom/refs/heads/main/security/tpg-telecom-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Telecommunications
- Australia
- Mobile Network Operator
- Broadband
- Messaging
- SMS
- IoT
- 5G
- Partner Gated
---
