---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: survata.com
  spf: true
hosts:
- cert_expires: Aug 31 21:52:06 2026 GMT
  host: www.survata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Survata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Survata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Survata
provider_slug: survata
slug: survata-domain-security
source_filename: survata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.survata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 21:52:06 2026 GMT\n  hsts: false\ndomains:\n- domain: survata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/survata/refs/heads/main/security/survata-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Market Research
- Survey
- Brand Measurement
- Advertising
- Analytics
---
