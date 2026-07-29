---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: thetrainline.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trainlinegroup.com
  spf: true
hosts:
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: www.thetrainline.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: www.trainlinegroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 13:08:21 2026 GMT
  host: tps.thetrainline.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Trainline Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trainline, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Trainline
provider_slug: trainline
slug: trainline-domain-security
source_filename: trainline-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thetrainline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.trainlinegroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tps.thetrainline.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 20 13:08:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thetrainline.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: trainlinegroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trainline/refs/heads/main/security/trainline-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Travel
- Rail
- United Kingdom
- Europe
- Booking
- Ticketing
- Distribution
- OTA
- Corporate Travel
---
