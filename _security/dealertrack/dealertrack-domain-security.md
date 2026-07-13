---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dealertrack.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coxautoinc.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: us.dealertrack.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: developer.coxautoinc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dealertrack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dealertrack, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dealertrack
provider_slug: dealertrack
slug: dealertrack-domain-security
source_filename: dealertrack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: us.dealertrack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: null\n- host: developer.coxautoinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: dealertrack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: coxautoinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dealertrack/refs/heads/main/security/dealertrack-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automotive
- Dealership
- DMS
- Dealer Management System
- F&I
- Credit Application
- Lender Network
- Cox Automotive
- Opentrack
- Partner Gated
---
