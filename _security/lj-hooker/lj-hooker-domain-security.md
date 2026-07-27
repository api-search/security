---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ljhooker.com.au
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ljhooker.co.nz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ljhcommercial.com.au
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ljhrural.com.au
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ljhland.com.au
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ljhooker.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ljx.com.au
  spf: true
hosts:
- cert_expires: Sep 14 19:24:58 2026 GMT
  host: www.ljhooker.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 08:11:11 2026 GMT
  host: www.ljhooker.co.nz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 03:23:50 2026 GMT
  host: www.ljhcommercial.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 20:01:04 2026 GMT
  host: www.ljhrural.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 15:46:35 2026 GMT
  host: www.ljhland.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: assets.ljhooker.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api01.ljx.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lj Hooker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LJ Hooker, probed live across 7 host(s) and 7 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LJ Hooker
provider_slug: lj-hooker
slug: lj-hooker-domain-security
source_filename: lj-hooker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of every LJ Hooker brand host in apis.yml/review.yml plus the vendor-operated\n  backend host api01.ljx.com.au\nhosts:\n- host: www.ljhooker.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:24:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.ljhooker.co.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:11:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.ljhcommercial.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 03:23:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.ljhrural.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 20:01:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.ljhland.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 15:46:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: assets.ljhooker.com\n  https: true\n\
  \  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: null\n- host: api01.ljx.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ljhooker.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: ljhooker.co.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: ljhcommercial.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: ljhrural.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: ljhland.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: ljhooker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: ljx.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lj-hooker/refs/heads/main/security/lj-hooker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- Australia
- New Zealand
- Property Listings
- Brokerage
- Property Management
- Rentals
- Commercial Real Estate
- PropTech
- Franchise
---
