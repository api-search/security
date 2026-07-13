---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:nso@uwo.ca"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uwo.ca
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scholaris.ca
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: www.uwo.ca
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  5 23:59:59 2027 GMT
  host: uwo.scholaris.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: wts.uwo.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Western Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Western University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Western University
provider_slug: western
slug: western-domain-security
source_filename: western-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uwo.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: false\n- host: uwo.scholaris.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wts.uwo.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uwo.ca\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:nso@uwo.ca\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: scholaris.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/western/refs/heads/main/security/western-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Canada
- Library
- Institutional Repository
- Open Access
- Identity
---
