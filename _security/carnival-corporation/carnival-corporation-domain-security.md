---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carnivalcorp.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: princess.com
  spf: true
hosts:
- cert_expires: Sep  8 02:44:02 2026 GMT
  host: www.carnivalcorp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.princess.com
  hsts: true
  hsts_max_age: 2628000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: www.carnival.com
  hsts: true
  hsts_max_age: 2628000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carnival Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carnival Corporation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Carnival Corporation
provider_slug: carnival-corporation
slug: carnival-corporation-domain-security
source_filename: carnival-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carnivalcorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 02:44:02 2026 GMT\n  hsts: false\n- host: www.princess.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2628000\n- host: www.carnival.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2628000\ndomains:\n- domain: carnivalcorp.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: princess.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carnival-corporation/refs/heads/main/security/carnival-corporation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cruise Lines
- Travel
- Hospitality
- Mobile Apps
- Loyalty
- Wearables
---
