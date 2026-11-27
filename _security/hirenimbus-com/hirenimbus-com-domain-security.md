---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hirenimbus.com
  spf: true
hosts:
- cert_expires: Feb  6 16:30:33 2027 GMT
  host: hirenimbus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HireNimbus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HireNimbus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HireNimbus
provider_slug: hirenimbus-com
slug: hirenimbus-com-domain-security
source_filename: hirenimbus-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hirenimbus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 16:30:33 2027 GMT\n  hsts: false\ndomains:\n- domain: hirenimbus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hirenimbus-com/security/hirenimbus-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Marketplace
- Home Services
- Professionals
- Booking
- United States
---
