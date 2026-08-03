---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: safe.security
  spf: true
- caa:
  - 0 issue "amazonaws.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "amazonaws.com"
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: false
  domain: balbix.net
  spf: true
- caa:
  - 0 issue "ssl.com"
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: balbix.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:_spf.salesforce.com include:3350762.spf07.hubspotemail.net include:mail.zendesk.com include:amazonses.com ~all
hosts:
- cert_expires: Sep 11 14:53:15 2026 GMT
  host: safe.security
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 01:02:14 2026 GMT
  host: docs.safe.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: app.balbix.net
  hsts: null
  https: true
  note: platform entry point; unauthenticated requests are redirected to the Okta authorization endpoint at login.balbix.net
  tls_version: TLSv1.3
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: login.balbix.net
  hsts: true
  hsts_max_age: 315360000
  https: true
  note: Okta-hosted identity provider for the Balbix platform
  tls_version: TLSv1.3
- cert_expires: Oct  9 14:49:59 2026 GMT
  host: www.balbix.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  http_status: 301
  https: true
  note: legacy Balbix marketing domain; issues HTTP 301 to https://safe.security/
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Balbix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Balbix, probed live across 5 host(s) and 3 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Balbix
provider_slug: balbix
slug: balbix-domain-security
source_filename: balbix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (script) plus manual probes of the\n  legacy balbix.com domain and the login.balbix.net identity host\nhosts:\n- host: safe.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 14:53:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.safe.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 01:02:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.balbix.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\n  note: platform entry point; unauthenticated requests are redirected to the Okta\n    authorization endpoint at login.balbix.net\n- host: login.balbix.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 315360000\n  note: Okta-hosted identity provider for the Balbix platform\n- host: www.balbix.com\n  https:\
  \ true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:49:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  http_status: 301\n  note: legacy Balbix marketing domain; issues HTTP 301 to https://safe.security/\ndomains:\n- domain: safe.security\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: balbix.net\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: false\n- domain: balbix.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n\
  \  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:_spf.salesforce.com\n    include:3350762.spf07.hubspotemail.net include:mail.zendesk.com\n    include:amazonses.com ~all\n  dmarc: true\n  dmarc_policy: none\nx-evidence:\n  fetched: '2026-08-02'\n  notes: DMARC policy on balbix.com is p=none (monitor only). balbix.net publishes no\n    DMARC record. Neither balbix.com nor balbix.net is DNSSEC-signed; safe.security is.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/balbix/refs/heads/main/security/balbix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Security
- Risk Management
- Vulnerability Management
- Exposure Management
- Asset Management
- Cyber Asset Attack Surface Management
- Continuous Threat Exposure Management
- Cyber Risk Quantification
- Application Security
---
