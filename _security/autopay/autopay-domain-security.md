---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild ";"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@autopay.io"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: autopay.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: autopay.no
  spf: true
hosts:
- cert_expires: Aug 13 12:37:23 2026 GMT
  host: developer.autopay.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- host: autopay.no
  https: false
- cert_expires: Sep  8 09:39:44 2026 GMT
  host: api.autopay.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autopay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autopay, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Autopay
provider_slug: autopay
slug: autopay-domain-security
source_filename: autopay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.autopay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 12:37:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: autopay.no\n  https: false\n- host: api.autopay.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 09:39:44 2026 GMT\n  hsts: null\ndomains:\n- domain: autopay.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \";\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@autopay.io\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: autopay.no\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autopay/refs/heads/main/security/autopay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Parking
- Parking Payments
- Fleet Management
- Permits
- Parking Operators
- Norway
---
