---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: enterprisemobility.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ehi.com
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.enterprisemobility.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  edge: Akamai
  host: developer.ehi.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15768000
  https: true
  note: 403s to browser-like user agents behind Akamai; serves 200 to a default curl user agent.
  tls_version: TLSv1.3
- cert_expires: Sep  8 23:59:59 2026 GMT
  edge: Imperva
  gateway: Kong Gateway
  host: api.ehi.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  https: true
  note: Production API gateway. Returns a JSON no-route 404 with a request_id to every anonymous path.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enterprise Mobility Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enterprise Mobility, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Enterprise Mobility
provider_slug: enterprise-mobility
slug: enterprise-mobility-domain-security
source_filename: enterprise-mobility-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of apis.yml hosts (0-working/probe-domain-security.py),\n  with the HSTS values re-verified by hand on 2026-07-28 — the script reported\n  null for all three hosts but every one of them does send\n  Strict-Transport-Security on both HEAD and GET.\nhosts:\n  - host: www.enterprisemobility.com\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Nov  7 23:59:59 2026 GMT\n    hsts: true\n    hsts_max_age: 15768000\n    hsts_include_subdomains: true\n  - host: developer.ehi.com\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Dec 19 23:59:59 2026 GMT\n    hsts: true\n    hsts_max_age: 15768000\n    hsts_include_subdomains: true\n    edge: Akamai\n    note: >-\n      403s to browser-like user agents behind Akamai; serves 200 to a default\n      curl user agent.\n  - host: api.ehi.com\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Sep  8 23:59:59 2026 GMT\n    hsts:\
  \ true\n    hsts_max_age: 31536000\n    hsts_include_subdomains: false\n    edge: Imperva\n    gateway: Kong Gateway\n    note: >-\n      Production API gateway. Returns a JSON no-route 404 with a request_id to\n      every anonymous path.\ndomains:\n  - domain: enterprisemobility.com\n    dnssec: false\n    caa: []\n    spf: true\n    dmarc: true\n    dmarc_policy: reject\n  - domain: ehi.com\n    dnssec: false\n    caa: []\n    spf: true\n    dmarc: true\n    dmarc_policy: reject\nsummary:\n  https_everywhere: true\n  tls13_everywhere: true\n  hsts_everywhere: true\n  dnssec: false\n  caa: false\n  spf: true\n  dmarc_reject: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enterprise-mobility/refs/heads/main/security/enterprise-mobility-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- United States
- Car Rental
- Ground Transportation
- Mobility
- Corporate Travel
- Distribution
- Fleet Management
- Insurance Replacement Rental
- Booking
---
