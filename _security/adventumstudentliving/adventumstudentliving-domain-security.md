---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: adventumstudentliving.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uniacco.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unicreds.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unischolars.com
  spf: false
hosts:
- cert_expires: Nov 16 21:35:55 2026 GMT
  host: adventumstudentliving.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: uniacco.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: unicreds.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: unischolars.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 4
kind: domain-security
layout: security
method: probed
name: Adventumstudentliving Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adventum Student Living, probed live across 4 host(s) and 4 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Adventum Student Living
provider_slug: adventumstudentliving
slug: adventumstudentliving-domain-security
source_filename: adventumstudentliving-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the ASL corporate domain and the four consumer brand hosts it links from adventumstudentliving.com\nnote: >-\n  adventumstudentliving.com is the corporate site; uniacco.com, unicreds.com and unischolars.com are\n  the operating brands ASL links from its own homepage and names in the UniAcco terms/privacy pages\n  (\"Adventum Student Living Private Limited, hereinafter also referred to as UniAcco\"). No API host\n  exists to probe — see well-known/adventumstudentliving-well-known.yml.\nhosts:\n- host: adventumstudentliving.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 16 21:35:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: uniacco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n- host: unicreds.com\n  https: true\n  tls_version: TLSv1.3\n\
  \  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: unischolars.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adventumstudentliving.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: uniacco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: unicreds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: unischolars.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adventumstudentliving/refs/heads/main/security/adventumstudentliving-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- Student Housing
- Study Abroad
- Real Estate
- Marketplace
- Lending
- Travel
- India
- Consumer
---
