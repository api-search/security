---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: m2pfintech.com
  spf: true
hosts:
- cert_expires: Aug 19 23:59:59 2026 GMT
  host: m2pfintech.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: M2P Fintech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for M2P Fintech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: M2P Fintech
provider_slug: m2p-fintech
slug: m2p-fintech-domain-security
source_filename: m2p-fintech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: m2pfintech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: m2pfintech.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/m2p-fintech/refs/heads/main/security/m2p-fintech-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fintech
- Banking
- Lending
- Payments
- Banking as a Service
- Card Issuing
- UPI
- KYC
- Cross-Border Payments
- Financial Infrastructure
---
