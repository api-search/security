---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bachatt.app
  spf: false
hosts:
- cert_expires: Oct 13 11:11:48 2026 GMT
  host: www.bachatt.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bachatt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bachatt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Bachatt
provider_slug: bachatt
slug: bachatt-domain-security
source_filename: bachatt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bachatt.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 11:11:48 2026 GMT\n  hsts: false\ndomains:\n- domain: bachatt.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bachatt/refs/heads/main/security/bachatt-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Savings
- Mutual Funds
- Investments
- Lending
- India
- Consumer Finance
---
