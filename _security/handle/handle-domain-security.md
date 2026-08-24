---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: handle.com
  spf: true
hosts:
- cert_expires: Nov 17 13:45:11 2026 GMT
  host: www.handle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 08:46:22 2026 GMT
  host: api.handle.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  note: Live API host. Root returns HTTP 404 "Cannot GET /" (Node/Express with Helmet security headers, served via Google Cloud); /api and /api/docs return a JSON route hint naming /api/integrations/{integration_name}/{action}.
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: app.handle.com
  hsts: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: Single-page application; every path returns HTTP 200 with the same 216,948-byte shell (soft-404 catch-all).
  tls_version: TLSv1.3
- cert_expires: Sep 25 16:09:59 2026 GMT
  host: trust.handle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: Vanta-hosted trust center (assets.vanta.com).
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Handle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Handle, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Handle
provider_slug: handle
slug: handle-domain-security
source_filename: handle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + the handle.com API/app/trust/status hosts\nhosts:\n- host: www.handle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 13:45:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.handle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 08:46:22 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  note: >-\n    Live API host. Root returns HTTP 404 \"Cannot GET /\" (Node/Express with Helmet security headers,\n    served via Google Cloud); /api and /api/docs return a JSON route hint naming\n    /api/integrations/{integration_name}/{action}.\n- host: app.handle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_preload: true\n  note: Single-page application; every path returns HTTP 200 with the same 216,948-byte shell (soft-404 catch-all).\n- host: trust.handle.com\n\
  \  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 16:09:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: Vanta-hosted trust center (assets.vanta.com).\ndomains:\n- domain: handle.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/handle/refs/heads/main/security/handle-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Construction
- Construction Finance
- Lien Management
- Lien Waivers
- Accounts Receivable
- Credit Management
- Payments
- B2B Payments
- Compliance
- ERP Integration
- Collections
- Financial Operations
- Material Suppliers
- Equipment Dealers
---
