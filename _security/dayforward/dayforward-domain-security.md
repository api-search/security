---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dayforward.io
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: dayforward.com
  spf: true
hosts:
- cert_expires: Oct 19 07:18:01 2026 GMT
  host: dayforward.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: www.dayforward.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 04:08:58 2026 GMT
  host: api.dayforward.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dayforward Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dayforward, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dayforward
provider_slug: dayforward
slug: dayforward-domain-security
source_filename: dayforward-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (dayforward.io, www.dayforward.com,\n  api.dayforward.com)\nhosts:\n- host: dayforward.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 07:18:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.dayforward.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n- host: api.dayforward.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 04:08:58 2026 GMT\n  hsts: false\ndomains:\n- domain: dayforward.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: dayforward.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nnotes:\n- The API host api.dayforward.com does not send Strict-Transport-Security, while both\n  web hosts do.\n- dayforward.io publishes no SPF and no DMARC record; dayforward.com publishes both,\n  but the DMARC policy is\
  \ p=none (monitor only, no enforcement).\n- Neither registrable domain publishes a CAA record.\n- dayforward.com is DNSSEC-signed; dayforward.io is not.\n- www.dayforward.com sends a strict Content-Security-Policy with frame-ancestors 'self',\n  object-src 'none' and upgrade-insecure-requests.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dayforward/refs/heads/main/security/dayforward-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Insurance
- Life Insurance
- Insurtech
- Financial-Services
- Underwriting
- Policy Administration
- Software-as-a-Service
- GraphQL
---
