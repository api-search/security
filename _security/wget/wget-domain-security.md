---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gnu.org
  spf: true
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@gitlab.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gitlab.com
  spf: true
hosts:
- cert_expires: Oct  7 10:16:19 2026 GMT
  host: www.gnu.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 08:56:37 2026 GMT
  host: ftp.gnu.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: gitlab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wget Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wget, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wget
provider_slug: wget
slug: wget-domain-security
source_filename: wget-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gnu.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 10:16:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ftp.gnu.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 08:56:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: gitlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gnu.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: gitlab.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@gitlab.com\"\n  spf: true\n\
  \  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wget/refs/heads/main/security/wget-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CLI
- Clients
- HTTP Client
- File Download
- Open Source
- GNU
---
