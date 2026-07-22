---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dogvacay.com
  spf: true
hosts:
- cert_expires: Oct 12 03:24:59 2026 GMT
  host: dogvacay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dogvacay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DogVacay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DogVacay
provider_slug: dogvacay
slug: dogvacay-domain-security
source_filename: dogvacay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dogvacay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:24:59 2026 GMT\n  hsts: false\ndomains:\n- domain: dogvacay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dogvacay/refs/heads/main/security/dogvacay-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Pet Care
- Marketplace
- Dog Boarding
- Pet Sitting
- Consumer
- Acquired
---
