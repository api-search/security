---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usefulsensors.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: moonshine.ai
  spf: false
hosts:
- cert_expires: Sep 14 10:00:26 2026 GMT
  host: usefulsensors.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 20:47:38 2026 GMT
  host: moonshine.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Useful Sensors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Useful Sensors, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Useful Sensors
provider_slug: useful-sensors
slug: useful-sensors-domain-security
source_filename: useful-sensors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usefulsensors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 10:00:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: moonshine.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:47:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usefulsensors.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: moonshine.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/useful-sensors/refs/heads/main/security/useful-sensors-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Speech To Text
- Text To Speech
- Voice
- Edge AI
- On-Device AI
- Machine Learning
- Open Source
---
