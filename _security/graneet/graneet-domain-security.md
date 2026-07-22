---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: graneet.com
  spf: false
hosts:
- cert_expires: Oct 16 14:32:53 2026 GMT
  host: www.graneet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Graneet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Graneet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Graneet
provider_slug: graneet
slug: graneet-domain-security
source_filename: graneet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.graneet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 14:32:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: graneet.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graneet/refs/heads/main/security/graneet-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Construction
- BTP
- ERP
- SaaS
- Invoicing
- Project Management
- Accounting
- Fintech
- France
---
