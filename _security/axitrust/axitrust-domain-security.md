---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: axitrust.com
  spf: true
hosts:
- cert_expires: Aug 27 20:07:18 2026 GMT
  host: www.axitrust.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axitrust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for axiTrust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: axiTrust
provider_slug: axitrust
slug: axitrust-domain-security
source_filename: axitrust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axitrust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 20:07:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: axitrust.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axitrust/refs/heads/main/security/axitrust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Insurance
- InsurTech
- Surety Bonds
- MSME
- India
- Government Procurement
---
