---
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "godaddy.com"
  - 0 issue "sectigo.com"
  - 0 issue "usertrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: whova.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zapier.com
  spf: true
hosts:
- cert_expires: Mar 18 15:26:05 2027 GMT
  host: whova.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: zapier.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whova Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whova, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Whova
provider_slug: whova
slug: whova-domain-security
source_filename: whova-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: whova.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 15:26:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: zapier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: whova.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"usertrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: zapier.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whova/refs/heads/main/security/whova-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Events
- Event Management
- Event App
- Registration
- Conferences
- Attendees
- Exhibitors
- Gated API
- Modeled
---
