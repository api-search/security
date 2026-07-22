---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aaaudi.com
  spf: false
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: aaaudi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aa Audience Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AA Audience, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AA Audience
provider_slug: aa-audience
slug: aa-audience-domain-security
source_filename: aa-audience-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aaaudi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: aaaudi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aa-audience/refs/heads/main/security/aa-audience-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Advertising
- Data
- Machine Learning
- Credit Scoring
- Financial Services
- Audience Targeting
- Adtech
---
