---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: ledgebrook.com
  spf: true
hosts:
- cert_expires: Sep 10 11:32:23 2026 GMT
  host: www.ledgebrook.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ledgebrook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ledgebrook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Ledgebrook
provider_slug: ledgebrook
slug: ledgebrook-domain-security
source_filename: ledgebrook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ledgebrook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 11:32:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ledgebrook.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ledgebrook/refs/heads/main/security/ledgebrook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Insurance
- Insurtech
- Excess and Surplus
- Specialty Insurance
- Managing General Agent
- Reinsurance
- Commercial Liability
- Cyber Insurance
- Underwriting
---
