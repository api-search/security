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
  dmarc_policy: reject
  dnssec: false
  domain: brightlocal.com
  spf: true
hosts:
- cert_expires: Sep 20 12:25:10 2026 GMT
  host: www.brightlocal.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 23:14:18 2026 GMT
  host: apidocs.brightlocal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 15:13:18 2026 GMT
  host: tools.brightlocal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brightlocal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrightLocal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BrightLocal
provider_slug: brightlocal
slug: brightlocal-domain-security
source_filename: brightlocal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brightlocal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 12:25:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: apidocs.brightlocal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:14:18 2026 GMT\n  hsts: false\n- host: tools.brightlocal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 15:13:18 2026 GMT\n  hsts: null\ndomains:\n- domain: brightlocal.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightlocal/refs/heads/main/security/brightlocal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Local SEO
- Business Listings
- Rank Tracking
- Reviews
- Citations
---
