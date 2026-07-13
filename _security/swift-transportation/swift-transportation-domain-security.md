---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: knight-swift.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: knighttrans.com
  spf: true
hosts:
- cert_expires: Sep 25 20:38:26 2026 GMT
  host: knight-swift.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:20:28 2026 GMT
  host: www.knighttrans.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swift Transportation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swift Transportation, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Swift Transportation
provider_slug: swift-transportation
slug: swift-transportation-domain-security
source_filename: swift-transportation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: knight-swift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 20:38:26 2026 GMT\n  hsts: false\n- host: www.knighttrans.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:20:28 2026 GMT\n  hsts: false\ndomains:\n- domain: knight-swift.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: knighttrans.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swift-transportation/refs/heads/main/security/swift-transportation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- EDI
- Freight
- Logistics
- Transportation
- Truckload
- Fortune 1000
---
