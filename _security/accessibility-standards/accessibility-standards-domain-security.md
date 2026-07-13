---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:sysreq@w3.org"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: w3.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: access-board.gov
  spf: true
hosts:
- cert_expires: Oct  7 03:48:25 2026 GMT
  host: www.w3.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 19:21:32 2026 GMT
  host: www.access-board.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 15:21:32 2026 GMT
  host: www.section508.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Accessibility Standards Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accessibility Standards, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Accessibility Standards
provider_slug: accessibility-standards
slug: accessibility-standards-domain-security
source_filename: accessibility-standards-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.w3.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 03:48:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.access-board.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 19:21:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.section508.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 15:21:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: w3.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:sysreq@w3.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: access-board.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accessibility-standards/refs/heads/main/security/accessibility-standards-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Accessibility
- Compliance
- UX
- Web Standards
- WCAG
- ARIA
- Section 508
- Disability
---
