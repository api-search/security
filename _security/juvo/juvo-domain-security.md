---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: juvo.com
  spf: true
hosts:
- cert_expires: Oct 17 07:14:21 2026 GMT
  host: juvo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Juvo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juvo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Juvo
provider_slug: juvo
slug: juvo-domain-security
source_filename: juvo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: juvo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 07:14:21 2026 GMT\n  hsts: null\ndomains:\n- domain: juvo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juvo/refs/heads/main/security/juvo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Financial Identity
- Credit Scoring
- Financial Services
- Mobile
- Underbanked
- Machine Learning
- Financial Inclusion
---
