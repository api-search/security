---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: everyaction.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: securevan.com
  spf: false
hosts:
- cert_expires: Sep  7 07:51:50 2026 GMT
  host: www.everyaction.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:28:55 2026 GMT
  host: docs.everyaction.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 15:56:09 2026 GMT
  host: api.securevan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bonterra Fka Everyaction Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bonterra (fka EveryAction), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bonterra (fka EveryAction)
provider_slug: bonterra-fka-everyaction
slug: bonterra-fka-everyaction-domain-security
source_filename: bonterra-fka-everyaction-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.everyaction.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 07:51:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.everyaction.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:28:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.securevan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:56:09 2026 GMT\n  hsts: false\ndomains:\n- domain: everyaction.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: securevan.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonterra-fka-everyaction/refs/heads/main/security/bonterra-fka-everyaction-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API
- CRM
- Nonprofit
- Fundraising
- Advocacy
- Political
- Voter Engagement
- Donor Management
- Organizing
---
