---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 15five.com
  spf: true
hosts:
- cert_expires: Aug 19 19:03:08 2026 GMT
  host: www.15five.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 23:10:48 2026 GMT
  host: my.15five.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 15Five Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 15Five, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 15Five
provider_slug: 15five
slug: 15five-domain-security
source_filename: 15five-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.15five.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 19:03:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: my.15five.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 23:10:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: 15five.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/15five/refs/heads/main/security/15five-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Performance Management
- Employee Engagement
- OKRs
- Check-ins
- HR
- Human Resources
- 1-on-1 Meetings
- Pulse Surveys
---
