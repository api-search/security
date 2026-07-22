---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: knowify.com
  spf: true
hosts:
- cert_expires: Sep 13 21:47:06 2026 GMT
  host: www.knowify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Knowify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knowify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Knowify
provider_slug: knowify
slug: knowify-domain-security
source_filename: knowify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.knowify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 21:47:06 2026 GMT\n  hsts: false\ndomains:\n- domain: knowify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knowify/refs/heads/main/security/knowify-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Construction
- Construction Management
- Job Costing
- Project Management
- Trade Contractors
- Field Service Management
- Service Dispatch
- Estimating
- AIA Billing
- Invoicing
- Time Tracking
- QuickBooks
- QuickBooks Online
- Intuit Enterprise Suite
- Zapier
- Construction SaaS
- Vertical SaaS
---
