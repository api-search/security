---
description: ''
domains:
- caa:
  - '0 iodef "mailto: alerts@testim.io"'
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: testim.io
  spf: true
hosts:
- cert_expires: Sep 13 15:13:15 2026 GMT
  host: www.testim.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 19:30:47 2026 GMT
  host: help.testim.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: api.testim.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Testim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Testim, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Testim
provider_slug: testim
slug: testim-domain-security
source_filename: testim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.testim.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 15:13:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.testim.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:30:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.testim.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: testim.io\n  dnssec: false\n  caa:\n  - '0 iodef \"mailto: alerts@testim.io\"'\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testim/refs/heads/main/security/testim-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Testing
- Test Automation
- QA
- AI Testing
- End-to-End Testing
- CI/CD
---
