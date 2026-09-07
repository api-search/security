---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: equifax.com
  spf: true
hosts:
- cert_expires: Nov  4 07:14:04 2026 GMT
  host: www.equifax.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: developer.equifax.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 25 23:59:59 2027 GMT
  host: api.equifax.com
  hsts: true
  hsts_max_age: 31536000
  hsts_note: 'Corrected by hand from a live HEAD https://api.equifax.com/ on 2026-09-06, which returned ''Strict-Transport-Security: max-age=31536000; includeSubDomains; preload''. probe-domain-security.py recorded null because the Apigee gateway answers its own root with HTTP 404, which raises in the script''s urllib path and skips header inspection - a false negative for any API host that 404s ''/''.'
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Equifax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Equifax, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Equifax
provider_slug: equifax
slug: equifax-domain-security
source_filename: equifax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.equifax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 07:14:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.equifax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.equifax.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_note: >-\n    Corrected by hand from a live HEAD https://api.equifax.com/ on 2026-09-06, which\n    returned 'Strict-Transport-Security: max-age=31536000; includeSubDomains; preload'.\n    probe-domain-security.py recorded null because the Apigee gateway answers its own\n    root with HTTP 404, which raises in the script's urllib path and skips header\n    inspection - a false negative for any API host that 404s '/'.\ndomains:\n\
  - domain: equifax.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equifax/refs/heads/main/security/equifax-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Credit
- Credit History
- Credit Reporting
- Identity
- Fraud Detection
- Fortune 1000
---
