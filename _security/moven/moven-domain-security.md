---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: moven.com
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: www.moven.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moven Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moven, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Moven
provider_slug: moven
slug: moven-domain-security
source_filename: moven-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moven.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: moven.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moven/refs/heads/main/security/moven-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Banking
- Financial Services
- Digital Banking
- Financial Wellness
- Banking as a Service
- SDK
- Analytics
---
