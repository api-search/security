---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 21gram.co.kr
  spf: true
hosts:
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: 21gram.co.kr
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 21Gram Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 21gram, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 21gram
provider_slug: 21gram
slug: 21gram-domain-security
source_filename: 21gram-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 21gram.co.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: 21gram.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/21gram/refs/heads/main/security/21gram-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Pet Care
- Pet Loss
- Funeral Services
- Consumer Services
- Booking
- Marketplace
- South Korea
---
