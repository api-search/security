---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yplanapp.com
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: yplanapp.com
  hsts: true
  hsts_max_age: 63115200
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Yplanapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for yplanapp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: yplanapp
provider_slug: yplanapp
slug: yplanapp-domain-security
source_filename: yplanapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yplanapp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63115200\ndomains:\n- domain: yplanapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yplanapp/refs/heads/main/security/yplanapp-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Events
- Event Discovery
- Ticketing
- Bookings
- Mobile
- Entertainment
---
