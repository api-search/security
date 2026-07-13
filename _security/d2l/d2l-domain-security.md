---
api_specs:
- filename: reference.html
  format: yaml
  label: Brightspace Learning Platform (LP) API
  slug: brightspace-lp-api
  spec_type: OpenAPI
  url: https://docs.valence.desire2learn.com/reference.html
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: d2l.com
  spf: true
- caa:
  - 0 iodef "mailto:soeplatform@d2l.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: true
  domain: desire2learn.com
  spf: true
hosts:
- cert_expires: Aug 17 15:35:15 2026 GMT
  host: www.d2l.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: docs.valence.desire2learn.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: D2L Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for D2L Brightspace, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: D2L Brightspace
provider_slug: d2l
slug: d2l-domain-security
source_filename: d2l-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.d2l.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 15:35:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.valence.desire2learn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: d2l.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: desire2learn.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:soeplatform@d2l.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d2l/refs/heads/main/security/d2l-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Learning Management System
- LMS
- Education Technology
- EdTech
- E-Learning
- Courses
- Grades
- Users
- Enrollments
- Quizzes
- Discussions
- Learning Outcomes
- ePortfolio
- SIS Integration
- LTI
---
