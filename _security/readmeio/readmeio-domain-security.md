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
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.com
  spf: true
hosts:
- cert_expires: Oct  6 16:29:30 2026 GMT
  host: readme.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 07:54:10 2026 GMT
  host: docs.readme.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 22:42:46 2026 GMT
  host: api.readme.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Readmeio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReadMe.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ReadMe.io
provider_slug: readmeio
slug: readmeio-domain-security
source_filename: readmeio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: readme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 16:29:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.readme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 07:54:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.readme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 22:42:46 2026 GMT\n  hsts: null\ndomains:\n- domain: readme.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/readmeio/refs/heads/main/security/readmeio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Apis
- Documentation
- API Documentation
- Developer Experience
- Developer Portal
- OpenAPI
- Developer Hub
- API Metrics
---
