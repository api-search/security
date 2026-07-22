---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: portal.com
  spf: false
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: www.portal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Portal Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Portal Software, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Portal Software
provider_slug: portal-software
slug: portal-software-domain-security
source_filename: portal-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.portal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: portal.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portal-software/refs/heads/main/security/portal-software-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Billing
- Revenue Management
- Defunct
- Acquired
- Oracle
---
