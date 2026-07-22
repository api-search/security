---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vacayhero.com
  spf: true
hosts:
- cert_expires: Oct  9 21:40:08 2026 GMT
  host: vacayhero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vacayhero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VacayHero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: VacayHero
provider_slug: vacayhero
slug: vacayhero-domain-security
source_filename: vacayhero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vacayhero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 21:40:08 2026 GMT\n  hsts: false\ndomains:\n- domain: vacayhero.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vacayhero/refs/heads/main/security/vacayhero-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Travel
- Hospitality
- Vacation Rentals
- Marketplace
- Venture Backed
- Acquired
---
