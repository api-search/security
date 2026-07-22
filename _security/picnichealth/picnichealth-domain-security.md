---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "certainly.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: picnichealth.com
  spf: true
hosts:
- cert_expires: Sep  6 19:59:27 2026 GMT
  host: picnichealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Picnichealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PicnicHealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: PicnicHealth
provider_slug: picnichealth
slug: picnichealth-domain-security
source_filename: picnichealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: picnichealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 19:59:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: picnichealth.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picnichealth/refs/heads/main/security/picnichealth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Digital Biology
- Health
- Medical Records
- Real-World Data
- Real-World Evidence
- HEOR
- OMOP
- Life Sciences
- Healthcare
---
