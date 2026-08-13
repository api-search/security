---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: digioh.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: lightboxcdn.com
  spf: true
hosts:
- cert_expires: Oct 28 02:07:08 2026 GMT
  host: www.digioh.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 15:05:41 2026 GMT
  host: help.digioh.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 03:29:48 2026 GMT
  host: www.lightboxcdn.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digioh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digioh, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Digioh
provider_slug: digioh
slug: digioh-domain-security
source_filename: digioh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digioh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 02:07:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.digioh.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:05:41 2026 GMT\n  hsts: false\n- host: www.lightboxcdn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 03:29:48 2026 GMT\n  hsts: null\ndomains:\n- domain: digioh.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lightboxcdn.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digioh/refs/heads/main/security/digioh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Marketing
- Ecommerce
- Personalization
- Zero-Party Data
- Forms
- Popups
- Quizzes
- Conversion Rate Optimization
- Identity Resolution
---
