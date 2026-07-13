---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: udemy.com
  spf: true
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 iodef "mailto:security@postman.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: postman.com
  spf: true
hosts:
- cert_expires: Sep 15 04:03:30 2026 GMT
  host: www.udemy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 09:00:12 2026 GMT
  host: www.postman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Udemy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Udemy, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Udemy
provider_slug: udemy
slug: udemy-domain-security
source_filename: udemy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.udemy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:03:30 2026 GMT\n  hsts: false\n- host: www.postman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 09:00:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: udemy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: postman.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 iodef \"mailto:security@postman.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/udemy/refs/heads/main/security/udemy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Online Learning
- E-Learning
- Education
- Courses
- Corporate Training
- Workforce Development
---
