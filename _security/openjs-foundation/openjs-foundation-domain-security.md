---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openjsf.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nodejs.org
  spf: true
hosts:
- cert_expires: Sep 21 01:59:51 2026 GMT
  host: openjsf.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: nodejs.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 04:03:06 2026 GMT
  host: expressjs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openjs Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenJS Foundation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenJS Foundation
provider_slug: openjs-foundation
slug: openjs-foundation-domain-security
source_filename: openjs-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openjsf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 01:59:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: nodejs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: expressjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 04:03:06 2026 GMT\n  hsts: false\ndomains:\n- domain: openjsf.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: nodejs.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openjs-foundation/refs/heads/main/security/openjs-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- JavaScript
- Linux Foundation
- Node.js
- Web
- API Frameworks
---
