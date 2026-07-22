---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: phoodsolutions.com
  spf: true
hosts:
- cert_expires: Sep 26 16:31:56 2026 GMT
  host: phoodsolutions.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phood Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phood Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Phood Solutions
provider_slug: phood-solutions
slug: phood-solutions-domain-security
source_filename: phood-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: phoodsolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:31:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: phoodsolutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phood-solutions/refs/heads/main/security/phood-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Food Waste
- Computer Vision
- Food Service
- Sustainability
- Analytics
- Restaurant Technology
---
