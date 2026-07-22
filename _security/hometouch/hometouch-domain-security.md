---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: myhometouch.com
  spf: false
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: myhometouch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hometouch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HomeTouch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: HomeTouch
provider_slug: hometouch
slug: hometouch-domain-security
source_filename: hometouch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: myhometouch.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: myhometouch.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hometouch/refs/heads/main/security/hometouch-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Health Care
- Home Care
- Elderly Care
- Dementia Care
- Care Marketplace
- United Kingdom
---
