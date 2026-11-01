---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tourmind.com
  spf: true
hosts:
- cert_expires: Apr 12 23:59:59 2027 GMT
  host: tourmind.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tourmind Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tourmind-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: tourmind-com
provider_slug: tourmind-com
slug: tourmind-com-domain-security
source_filename: tourmind-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tourmind.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Apr 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: tourmind.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/tourmind-com/security/tourmind-com-domain-security.yml
summary_line: TLSv1.2
tags:
- Travel
- AI
- Booking
- SaaS
- B2B
---
