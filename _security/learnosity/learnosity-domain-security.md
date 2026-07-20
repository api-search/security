---
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: learnosity.com
  spf: true
hosts:
- cert_expires: Sep 18 23:40:27 2026 GMT
  host: help.learnosity.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 17:19:26 2026 GMT
  host: learnosity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: data.learnosity.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Learnosity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Learnosity, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Learnosity
provider_slug: learnosity
slug: learnosity-domain-security
source_filename: learnosity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: help.learnosity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:40:27 2026 GMT\n  hsts: null\n- host: learnosity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:19:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: data.learnosity.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: learnosity.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/learnosity/refs/heads/main/security/learnosity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Assessment
- EdTech
- Learning
- Analytics
- Content Authoring
- Artificial Intelligence
- Accessibility
- Company
---
