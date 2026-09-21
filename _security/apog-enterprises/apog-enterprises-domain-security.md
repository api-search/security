---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apog.com
  spf: false
hosts:
- cert_expires: Oct 27 02:44:40 2026 GMT
  host: www.apog.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.apog.com
  https: false
- host: api.apog.com
  https: false
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Apog Enterprises Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apogee Enterprises, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Apogee Enterprises
provider_slug: apog-enterprises
slug: apog-enterprises-domain-security
source_filename: apog-enterprises-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apog.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 02:44:40 2026 GMT\n  hsts: null\n- host: developer.apog.com\n  https: false\n- host: api.apog.com\n  https: false\ndomains:\n- domain: apog.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apog-enterprises/refs/heads/main/security/apog-enterprises-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Glass
- Architectural Glass
- Architectural Framing
- Storefront Systems
- Curtain Wall
- Building Products
- Construction
- Investor Relations
- Fortune 1000
---
