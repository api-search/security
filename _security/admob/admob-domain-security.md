---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Sep 21 08:37:24 2026 GMT
  host: admob.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:37:24 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 08:39:19 2026 GMT
  host: admob.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Admob Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AdMob, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AdMob
provider_slug: admob
slug: admob-domain-security
source_filename: admob-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: admob.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:37:24 2026 GMT\n  hsts: false\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:37:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: admob.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 08:39:19 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/admob/refs/heads/main/security/admob-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Mobile
- Monetization
- Ads
- Google
- Reporting
- Mediation
- AdTech
---
