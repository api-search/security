---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: beautydate.com.br
  spf: true
hosts:
- cert_expires: Sep 21 21:17:17 2026 GMT
  host: beautydate.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beautydate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BeautyDate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BeautyDate
provider_slug: beautydate
slug: beautydate-domain-security
source_filename: beautydate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beautydate.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 21:17:17 2026 GMT\n  hsts: null\ndomains:\n- domain: beautydate.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beautydate/refs/heads/main/security/beautydate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Beauty
- Booking
- Scheduling
- Appointments
- Marketplace
- Brazil
- Wellness
---
