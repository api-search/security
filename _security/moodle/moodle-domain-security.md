---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: moodledev.io
  spf: false
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moodle.org
  spf: true
hosts:
- cert_expires: Aug 27 15:03:49 2026 GMT
  host: moodledev.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 11:14:51 2026 GMT
  host: moodle.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moodle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moodle, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Moodle
provider_slug: moodle
slug: moodle-domain-security
source_filename: moodle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moodledev.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 15:03:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: moodle.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 11:14:51 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: moodledev.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: moodle.org\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moodle/refs/heads/main/security/moodle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Learning
- EdTech
- LMS
- Moodle
- Open Source
- Web Services
---
