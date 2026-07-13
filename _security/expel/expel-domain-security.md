---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: expel.com
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: expel.io
  spf: true
hosts:
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: expel.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 28 10:47:47 2026 GMT
  host: workbench.expel.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Expel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Expel, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Expel
provider_slug: expel
slug: expel-domain-security
source_filename: expel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: expel.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: workbench.expel.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 10:47:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: expel.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: expel.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expel/refs/heads/main/security/expel-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Cybersecurity
- MDR
- Managed Detection and Response
- SOC
- SIEM
- Workbench
---
