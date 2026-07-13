---
api_specs:
- filename: openapi.json
  format: json
  label: Procurify API
  slug: procurify-api
  spec_type: OpenAPI
  url: https://developer.procurify.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: procurify.com
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.procurify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 07:17:13 2026 GMT
  host: developer.procurify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.procurify.com
  https: false
kind: domain-security
layout: security
method: probed
name: Procurify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Procurify, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Procurify
provider_slug: procurify
slug: procurify-domain-security
source_filename: procurify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.procurify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: false\n- host: developer.procurify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 07:17:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.procurify.com\n  https: false\ndomains:\n- domain: procurify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/procurify/refs/heads/main/security/procurify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Spend Management
- Procurement
- Purchase Orders
- Accounts Payable
- Vendor Management
- Budget Tracking
- Procure-to-Pay
- ERP Integration
---
