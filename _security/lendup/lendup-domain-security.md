---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lendup.com
  spf: true
hosts:
- cert_expires: Sep 14 06:30:51 2026 GMT
  host: lendup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lendup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LendUp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LendUp
provider_slug: lendup
slug: lendup-domain-security
source_filename: lendup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lendup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 06:30:51 2026 GMT\n  hsts: false\ndomains:\n- domain: lendup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lendup/refs/heads/main/security/lendup-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Consumer Lending
- Fintech
- Financial Services
- Personal Loans
- Lead Generation
- Defunct
---
