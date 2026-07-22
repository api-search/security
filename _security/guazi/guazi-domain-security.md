---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: guazi.com
  spf: true
hosts:
- cert_expires: Mar 31 02:31:16 2027 GMT
  host: guazi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Guazi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guazi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Guazi
provider_slug: guazi
slug: guazi-domain-security
source_filename: guazi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: guazi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 31 02:31:16 2027 GMT\n  hsts: false\ndomains:\n- domain: guazi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guazi/refs/heads/main/security/guazi-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Technology
- Automotive
- Used Cars
- Marketplace
- E-Commerce
- Auctions
- Logistics
- China
---
