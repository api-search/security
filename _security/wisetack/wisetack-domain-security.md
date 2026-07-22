---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wisetack.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wisetack.us
  spf: true
hosts:
- cert_expires: Oct  2 05:40:17 2026 GMT
  host: www.wisetack.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: api.wisetack.us
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wisetack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wisetack, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wisetack
provider_slug: wisetack
slug: wisetack-domain-security
source_filename: wisetack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wisetack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:40:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wisetack.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wisetack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wisetack.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wisetack/refs/heads/main/security/wisetack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Lending
- Consumer Financing
- Embedded Finance
- Payments
- Home Services
---
