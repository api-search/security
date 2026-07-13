---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: franconnect.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: franconnect.net
  spf: false
hosts:
- cert_expires: Sep  5 22:29:20 2026 GMT
  host: www.franconnect.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: docs.franconnect.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Franconnect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FranConnect, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FranConnect
provider_slug: franconnect
slug: franconnect-domain-security
source_filename: franconnect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.franconnect.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 22:29:20 2026 GMT\n  hsts: false\n- host: docs.franconnect.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: franconnect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: franconnect.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/franconnect/refs/heads/main/security/franconnect-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Franchise Management
- Franchise Development
- Franchise Operations
- Field Operations
- Multi-Location
- CRM
- Franchise Sales
- SaaS
---
