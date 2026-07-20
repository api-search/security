---
api_specs:
- filename: spendesk-public-api
  format: yaml
  label: Spendesk Public API
  slug: spendesk-public-api
  spec_type: Postman
  url: https://www.postman.com/spendesk-pde-sas/spendesk-public-api/collection/q48314q/spendesk-public-api
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: spendesk.com
  spf: true
hosts:
- cert_expires: Aug 14 08:53:49 2026 GMT
  host: www.spendesk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:40:30 2026 GMT
  host: developer.spendesk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: api.spendesk.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Spendesk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spendesk, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Spendesk
provider_slug: spendesk
slug: spendesk-domain-security
source_filename: spendesk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spendesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 08:53:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.spendesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:40:30 2026 GMT\n  hsts: null\n- host: api.spendesk.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: spendesk.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spendesk/refs/heads/main/security/spendesk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Spend Management
- Corporate Cards
- Expense Management
- Invoices
- Procurement
- FinTech
- Accounting
- Payments
---
