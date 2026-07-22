---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: truefort.com
  mx:
  - truefort-com.mail.protection.outlook.com
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com include:_spf.salesforce.com include:m.lessonly.com include:_spf.psm.knowbe4.com -all
hosts:
- host: truefort.com
  hsts: null
  http_port_80_status: 409
  https: null
  tls_probe: handshake-rejected (TLS alert 40; edge blocks non-browser TLS fingerprints)
- host: www.truefort.com
  hsts: null
  https: null
  tls_probe: handshake-rejected (TLS alert 40; edge blocks non-browser TLS fingerprints)
kind: domain-security
layout: security
method: probed
name: Truefort Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TrueFort, probed live across 2 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TrueFort
provider_slug: truefort
slug: truefort-domain-security
source_filename: truefort-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: dig + TLS/HTTP probes (API Evangelist enrichment pipeline)\nnote: >-\n  TrueFort ceased operations on 2025-05-21 (shutdown notice on truefort.com).\n  The marketing site remains online behind a WP Engine edge that rejects\n  non-browser TLS clients (handshake alert 40 for curl/LibreSSL, OpenSSL,\n  and Python probes; plain HTTP on port 80 answers 409), so HTTPS/TLS/HSTS\n  fields could not be observed from this vantage even though the site is\n  reachable in browsers and by archive crawlers. DNS records were probed\n  directly and are authoritative.\nhosts:\n  - host: truefort.com\n    https: null\n    tls_probe: handshake-rejected (TLS alert 40; edge blocks non-browser TLS fingerprints)\n    http_port_80_status: 409\n    hsts: null\n  - host: www.truefort.com\n    https: null\n    tls_probe: handshake-rejected (TLS alert 40; edge blocks non-browser TLS fingerprints)\n    hsts: null\ndomains:\n  - domain: truefort.com\n    dnssec:\
  \ false\n    caa: []\n    spf: true\n    spf_record: 'v=spf1 include:spf.protection.outlook.com include:_spf.salesforce.com\n      include:m.lessonly.com include:_spf.psm.knowbe4.com -all'\n    dmarc: false\n    mx:\n      - truefort-com.mail.protection.outlook.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truefort/refs/heads/main/security/truefort-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Cybersecurity
- Microsegmentation
- Zero Trust
- Lateral Movement
- Workload Security
- Service Accounts
- Defunct
---
