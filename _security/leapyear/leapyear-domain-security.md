---
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: leapyear.io
  nameservers: markmonitor.com
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: readthedocs-hosted.com
  spf: false
hosts:
- a_record: 3.33.139.32
  host: leapyear.io
  hsts: null
  https: false
  result: connection timed out after 8s
  tls_version: null
- a_record: 3.33.139.32
  host: www.leapyear.io
  https: false
  result: connection timed out after 8s
- a_record: 3.33.139.32
  host: docs.leapyear.io
  https: false
  result: connection timed out after 8s
- cert_expires: Aug 21 18:43:48 2026 GMT
  host: leapyear-python-docs.readthedocs-hosted.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leapyear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeapYear, probed live across 4 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LeapYear
provider_slug: leapyear
slug: leapyear-domain-security
source_filename: leapyear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnotes: >-\n  The readthedocs-hosted docs host is the only reachable LeapYear developer surface;\n  its posture is the hosting provider's, not LeapYear's. The corporate domain\n  leapyear.io still resolves and is still held on MarkMonitor nameservers after the\n  Snowflake acquisition, but it serves nothing and publishes no CAA, SPF or DMARC.\nhosts:\n- host: leapyear.io\n  https: false\n  result: connection timed out after 8s\n  a_record: 3.33.139.32\n  tls_version: null\n  hsts: null\n- host: www.leapyear.io\n  https: false\n  result: connection timed out after 8s\n  a_record: 3.33.139.32\n- host: docs.leapyear.io\n  https: false\n  result: connection timed out after 8s\n  a_record: 3.33.139.32\n- host: leapyear-python-docs.readthedocs-hosted.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 18:43:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n\
  - domain: leapyear.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  nameservers: markmonitor.com\n- domain: readthedocs-hosted.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leapyear/refs/heads/main/security/leapyear-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Data Privacy
- Differential Privacy
- Machine Learning
- Analytics
- Data Clean Rooms
- Privacy Enhancing Technologies
- Python
- Acquired
---
