---
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: conga.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: congacloud.io
  spf: true
hosts:
- cert_expires: Aug  5 01:12:48 2026 GMT
  host: www.conga.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 11:31:16 2026 GMT
  host: developer.conga.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: rlp-dev.congacloud.io
  https: false
kind: domain-security
layout: security
method: probed
name: Conga Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conga, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Conga
provider_slug: conga
slug: conga-domain-security
source_filename: conga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conga.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  5 01:12:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.conga.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 11:31:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rlp-dev.congacloud.io\n  https: false\ndomains:\n- domain: conga.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: congacloud.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conga/refs/heads/main/security/conga-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise Software
- Contract Lifecycle Management
- CPQ
- Revenue Lifecycle Management
- Document Automation
- E-Signature
- Contract Intelligence
- CRM
---
