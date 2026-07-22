---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: outpostnow.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: outpostanywhere.com
  spf: false
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: outpostnow.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: api.outpostanywhere.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- host: partner.outpostanywhere.com
  https: false
kind: domain-security
layout: security
method: probed
name: Outpost Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Outpost, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Outpost
provider_slug: outpost
slug: outpost-domain-security
source_filename: outpost-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: outpostnow.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: false\n- host: api.outpostanywhere.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: null\n- host: partner.outpostanywhere.com\n  https: false\ndomains:\n- domain: outpostnow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: outpostanywhere.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outpost/refs/heads/main/security/outpost-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Merchant of Record
- Tax of Record
- Cross-Border Commerce
- Payments
- Tax Compliance
- E-Commerce
- VAT
- Fintech
- Invoicing
- Onboarding
---
