---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lastminute.com
  spf: true
hosts:
- cert_expires: Sep  7 09:53:25 2026 GMT
  host: www.lastminute.com
  hsts: null
  https: true
  notes: consumer storefront; returns 403 to non-browser clients (bot protection)
  tls_version: TLSv1.3
- cert_expires: Aug 31 01:11:16 2026 GMT
  host: developers.lastminute.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  notes: Stoplight-hosted API portal
- cert_expires: Sep  8 20:40:52 2026 GMT
  host: corporate.lastminute.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  notes: corporate/investor site (WordPress)
- cert_expires: Nov  3 23:59:59 2026 GMT
  host: technology.lastminute.com
  hsts: null
  https: true
  notes: engineering blog; no HSTS header observed
kind: domain-security
layout: security
method: probed
name: Lastminute Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lastminute.com, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: lastminute.com
provider_slug: lastminute-com
slug: lastminute-com-domain-security
source_filename: lastminute-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (base probe extended by hand to\n  the developer-portal, corporate and technology hosts)\nhosts:\n- host: www.lastminute.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 09:53:25 2026 GMT\n  hsts: null\n  notes: consumer storefront; returns 403 to non-browser clients (bot protection)\n- host: developers.lastminute.com\n  https: true\n  cert_expires: Aug 31 01:11:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  notes: Stoplight-hosted API portal\n- host: corporate.lastminute.com\n  https: true\n  cert_expires: Sep  8 20:40:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  notes: corporate/investor site (WordPress)\n- host: technology.lastminute.com\n  https: true\n  cert_expires: Nov  3 23:59:59 2026 GMT\n  hsts: null\n  notes: engineering blog; no HSTS header observed\n\
  domains:\n- domain: lastminute.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lastminute-com/refs/heads/main/security/lastminute-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Travel
- Online Travel Agency
- Flights
- Hotels
- Holiday Packages
- Travel Tech
- E-Commerce
- Europe
---
