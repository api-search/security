---
description: ''
domains:
- caa:
  - 128 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 128 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swiftconnect.com
  spf: true
- caa:
  - 128 issue "letsencrypt.org"
  - 128 issuewild "letsencrypt.org"
  - 0 issue "digicert.com"
  - 128 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swiftconnect.io
  note: Registrable domain of the API host (api.swiftconnect.io). Added by hand from live dig output because the script derived domains from the Website host only; DMARC here is strict (p=reject, pct=100, adkim=s, aspf=s).
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Oct 17 17:41:49 2026 GMT
  host: www.swiftconnect.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: swiftconnect.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 20 06:02:34 2026 GMT
  host: api.swiftconnect.io
  hsts: null
  hsts_note: 'The script probes the host root, which is answered by a plain-text 404 handler that emits no security headers. A request to a real API route DOES return `strict-transport-security: max-age=31536000; includeSubDomains`, alongside `x-content-type-options: nosniff`, `x-frame-options: DENY` and `permissions-policy: interest-cohort=()`. Observed 2026-08-29 on https://api.swiftconnect.io/credentials (HTTP 401).'
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swiftconnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SwiftConnect, probed live across 3 host(s) and 3 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SwiftConnect
provider_slug: swiftconnect
slug: swiftconnect-domain-security
source_filename: swiftconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swiftconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 17:41:49 2026 GMT\n  hsts: false\n- host: swiftconnect.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.swiftconnect.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 06:02:34 2026 GMT\n  hsts: null\n  hsts_note: >-\n    The script probes the host root, which is answered by a plain-text 404 handler that emits no\n    security headers. A request to a real API route DOES return\n    `strict-transport-security: max-age=31536000; includeSubDomains`, alongside\n    `x-content-type-options: nosniff`, `x-frame-options: DENY` and\n    `permissions-policy: interest-cohort=()`. Observed 2026-08-29 on\n    https://api.swiftconnect.io/credentials (HTTP 401).\ndomains:\n- domain:\
  \ swiftconnect.com\n  dnssec: false\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 128 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: swiftconnect.io\n  dnssec: false\n  caa:\n  - 128 issue \"letsencrypt.org\"\n  - 128 issuewild \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 128 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  note: >-\n    Registrable domain of the API host (api.swiftconnect.io). Added by hand from live dig output\n    because the script derived domains from the Website host only; DMARC here is strict\n    (p=reject, pct=100, adkim=s, aspf=s).\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swiftconnect/refs/heads/main/security/swiftconnect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Access Control
- Physical Security
- Identity
- Credentials
- Mobile Wallet
- Workplace
- Commercial Real Estate
- Provisioning
- Internet of Things
---
