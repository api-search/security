---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adroll.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nextroll.com
  spf: true
hosts:
- cert_expires: Sep  1 20:08:07 2026 GMT
  host: www.adroll.com
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: apidocs.nextroll.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: services.adroll.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Adroll Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdRoll, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AdRoll
provider_slug: adroll
slug: adroll-domain-security
source_filename: adroll-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adroll.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  1 20:08:07 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\n- host: apidocs.nextroll.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: services.adroll.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: adroll.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nextroll.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adroll/refs/heads/main/security/adroll-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Advertising
- Display Advertising
- Retargeting
- Marketing
- AdTech
- Programmatic
---
