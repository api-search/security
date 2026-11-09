---
description: ''
domains:
- caa:
  - 0 issuewild "sectigo.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adrenalinelist.com
  spf: false
hosts:
- cert_expires: Jan 27 07:23:34 2027 GMT
  host: adrenalinelist.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adrenalinelist Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adrenaline List, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Adrenaline List
provider_slug: adrenalinelist-com
slug: adrenalinelist-com-domain-security
source_filename: adrenalinelist-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adrenalinelist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 07:23:34 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adrenalinelist.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/adrenalinelist-com/security/adrenalinelist-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Adventure
- Bucket-List
- Travel
- Extreme-Sports
- Community
---
