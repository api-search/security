---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: darktrace.com
  spf: true
hosts:
- cert_expires: Oct  7 23:18:51 2026 GMT
  host: www.darktrace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 09:43:50 2026 GMT
  host: customerportal.darktrace.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: customer-instance.cloud.darktrace.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Darktrace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Darktrace, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Darktrace
provider_slug: darktrace
slug: darktrace-domain-security
source_filename: darktrace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.darktrace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:18:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: customerportal.darktrace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 09:43:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: customer-instance.cloud.darktrace.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: darktrace.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/darktrace/refs/heads/main/security/darktrace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cybersecurity
- Self-Learning AI
- ActiveAI
- NDR
- Email Security
- Cloud Security
- OT Security
- Endpoint Security
---
