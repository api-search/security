---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swiftnav.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: buf.build
  spf: true
hosts:
- cert_expires: Oct 23 12:36:45 2026 GMT
  host: www.swiftnav.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- host: na.all-freq.skylark.swiftnav.com
  https: false
- cert_expires: Nov 15 02:06:32 2026 GMT
  host: buf.build
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swift Navigation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swift Navigation, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Swift Navigation
provider_slug: swift-navigation
slug: swift-navigation-domain-security
source_filename: swift-navigation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swiftnav.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 12:36:45 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: na.all-freq.skylark.swiftnav.com\n  https: false\n- host: buf.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 02:06:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: swiftnav.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: buf.build\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swift-navigation/refs/heads/main/security/swift-navigation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- GNSS
- Precise Positioning
- Location
- Corrections
- RTK
- NTRIP
- RTCM
- Automotive
- Geospatial
- IoT
- Robotics
- Protocols
---
