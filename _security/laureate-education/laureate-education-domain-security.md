---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: laureate.net
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: uvm.mx
  spf: true
hosts:
- cert_expires: Aug 16 17:02:51 2026 GMT
  host: www.laureate.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 00:30:46 2026 GMT
  host: uvm.mx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 16:42:55 2026 GMT
  host: www.unitec.mx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Laureate Education Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laureate Education, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Laureate Education
provider_slug: laureate-education
slug: laureate-education-domain-security
source_filename: laureate-education-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.laureate.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 17:02:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: uvm.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 00:30:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.unitec.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:42:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: laureate.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: uvm.mx\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laureate-education/refs/heads/main/security/laureate-education-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- For Profit Education
- University Network
- Mexico
- Peru
- Latin America
- Private Equity
- B Corporation
- Take Private
---
