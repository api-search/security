---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: shearshare.com
  spf: true
hosts:
- cert_expires: Aug 11 05:46:24 2026 GMT
  host: shearshare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shearshare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShearShare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ShearShare
provider_slug: shearshare
slug: shearshare-domain-security
source_filename: shearshare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shearshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 05:46:24 2026 GMT\n  hsts: false\ndomains:\n- domain: shearshare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shearshare/refs/heads/main/security/shearshare-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Marketplace
- Beauty
- Salon
- Barbershop
- Booth Rental
- Space as a Service
- Gig Economy
- Mobile App
---
