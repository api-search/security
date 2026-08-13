---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: madvertise.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: bluestack.app
  spf: false
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: madvertise.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: developers.bluestack.app
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: mobile.mng-ads.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Madvertise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Madvertise, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Madvertise
provider_slug: madvertise
slug: madvertise-domain-security
source_filename: madvertise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: madvertise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\n- host: developers.bluestack.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: false\n- host: mobile.mng-ads.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: madvertise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: bluestack.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madvertise/refs/heads/main/security/madvertise-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Advertising
- AdTech
- Mobile
- Monetization
- Programmatic
- OpenRTB
- SDK
- Publishers
---
