---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: olist.com
  spf: true
hosts:
- cert_expires: Jul 28 19:28:41 2026 GMT
  host: olist.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Olist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Olist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Olist
provider_slug: olist
slug: olist-domain-security
source_filename: olist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: olist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 19:28:41 2026 GMT\n  hsts: false\ndomains:\n- domain: olist.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/olist/refs/heads/main/security/olist-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-commerce
- Marketplace
- Payments
- Logistics
- ERP
- Brazil
- Commerce
- Integration
---
