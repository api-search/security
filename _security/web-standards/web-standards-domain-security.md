---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: w3.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: whatwg.org
  spf: true
hosts:
- cert_expires: Oct  7 03:48:25 2026 GMT
  host: www.w3.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 02:20:30 2026 GMT
  host: whatwg.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  6 21:30:55 2026 GMT
  host: ietf.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Web Standards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Web Standards, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Web Standards
provider_slug: web-standards
slug: web-standards-domain-security
source_filename: web-standards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.w3.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:48:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: whatwg.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 23 02:20:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ietf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 21:30:55 2026 GMT\n  hsts: false\ndomains:\n- domain: w3.org\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: whatwg.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/web-standards/refs/heads/main/security/web-standards-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Browser Compatibility
- CSS
- HTML
- Interoperability
- JavaScript
- Standards
- Web APIs
- Web Development
---
