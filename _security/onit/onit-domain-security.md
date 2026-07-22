---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: onitbank.com
  spf: true
hosts:
- cert_expires: Oct 18 01:13:30 2026 GMT
  host: onitbank.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Onit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Onit
provider_slug: onit
slug: onit-domain-security
source_filename: onit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onitbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 01:13:30 2026 GMT\n  hsts: null\ndomains:\n- domain: onitbank.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onit/refs/heads/main/security/onit-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fintech
- Neobank
- Banking
- Payments
- Mobile Money
- Kenya
- Africa
- Microfinance
- Financial Services
---
