---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: true
  domain: cdnjs.com
  spf: true
hosts:
- cert_expires: Oct  7 00:57:38 2026 GMT
  host: api.cdnjs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cdnjs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CDNJS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: CDNJS
provider_slug: cdnjs
slug: cdnjs-domain-security
source_filename: cdnjs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.cdnjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:57:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cdnjs.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cdnjs/refs/heads/main/security/cdnjs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Development
- Public APIs
---
