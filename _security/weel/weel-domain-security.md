---
api_specs:
- filename: weel-openapi.yml
  format: yaml
  label: Weel Open API
  slug: weel-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/openapi/weel-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: letsweel.com
  spf: true
hosts:
- cert_expires: Sep 15 01:49:52 2026 GMT
  host: letsweel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 15:26:00 2026 GMT
  host: developer.letsweel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: public.letsweel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weel, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Weel
provider_slug: weel
slug: weel-domain-security
source_filename: weel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: letsweel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:49:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.letsweel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 15:26:00 2026 GMT\n  hsts: false\n- host: public.letsweel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: letsweel.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weel/refs/heads/main/security/weel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Australia
- Spend Management
- Expense Management
- Corporate Cards
- Accounts Payable
- Card Issuing
- Reimbursements
- Budgets
- Fintech
---
