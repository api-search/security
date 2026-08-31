---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: appliedsystems.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: myappliedproducts.com
  spf: true
hosts:
- cert_expires: Sep  6 02:56:48 2026 GMT
  host: www.appliedsystems.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 00:01:43 2026 GMT
  host: devcenter.myappliedproducts.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 14:20:40 2026 GMT
  host: api.myappliedproducts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Applied Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Applied Systems, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Applied Systems
provider_slug: applied-systems
slug: applied-systems-domain-security
source_filename: applied-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.appliedsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 02:56:48 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: devcenter.myappliedproducts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 00:01:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: api.myappliedproducts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 14:20:40 2026 GMT\n  hsts: null\ndomains:\n- domain: appliedsystems.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: myappliedproducts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applied-systems/refs/heads/main/security/applied-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- InsurTech
- Agency Management
- Applied Epic
- CRM
- Policy Management
- Partner Gated
---
