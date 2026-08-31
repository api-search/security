---
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ivanti.com
  spf: true
hosts:
- cert_expires: Oct  5 00:49:15 2026 GMT
  host: www.ivanti.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 00:49:15 2026 GMT
  host: help.ivanti.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 00:49:15 2026 GMT
  host: forums.ivanti.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ivanti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ivanti, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ivanti
provider_slug: ivanti
slug: ivanti-domain-security
source_filename: ivanti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ivanti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:49:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.ivanti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:49:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: forums.ivanti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 00:49:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ivanti.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ivanti/refs/heads/main/security/ivanti-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Endpoint Management
- IT Asset Management
- IT Service Management
- Patch Management
- Mobile Device Management
- Zero Trust
---
