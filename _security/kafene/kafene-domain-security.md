---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kafene.com
  spf: true
hosts:
- cert_expires: Sep 19 17:17:24 2026 GMT
  host: www.kafene.com
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 08:13:02 2026 GMT
  host: merchant.kafene.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 7776000
  https: true
  note: merchant portal single-page app; returns 200 HTML for every path (SPA catch-all)
  tls_version: TLSv1.3
- cert_expires: Oct 25 08:13:02 2026 GMT
  host: application.kafene.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 7776000
  https: true
  note: consumer lease application / dashboard SPA; SPA catch-all on every path
  tls_version: TLSv1.3
- cert_expires: Oct 25 08:13:02 2026 GMT
  host: app.kafene.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 08:13:02 2026 GMT
  host: customer.kafene.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- host: api.kafene.com
  http_status: 530
  https: true
  note: 'DNS resolves to Cloudflare but the edge returns "error code: 1016" (origin DNS error) for every path probed (/, /openapi.json, /swagger.json, /docs, /health). No origin is currently serving this hostname.'
  reachable: false
kind: domain-security
layout: security
method: probed
name: Kafene Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kafene, probed live across 6 host(s) and 1 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 5 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kafene
provider_slug: kafene
slug: kafene-domain-security
source_filename: kafene-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + discovered kafene.com subdomains\nhosts:\n- host: www.kafene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 17:17:24 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: merchant.kafene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 08:13:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n  hsts_include_subdomains: true\n  note: merchant portal single-page app; returns 200 HTML for every path (SPA catch-all)\n- host: application.kafene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 08:13:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n  hsts_include_subdomains: true\n  note: consumer lease application / dashboard SPA; SPA catch-all on every path\n- host: app.kafene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 08:13:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n  hsts_include_subdomains:\
  \ true\n- host: customer.kafene.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 08:13:02 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n  hsts_include_subdomains: true\n- host: api.kafene.com\n  https: true\n  reachable: false\n  http_status: 530\n  note: >-\n    DNS resolves to Cloudflare but the edge returns \"error code: 1016\" (origin DNS\n    error) for every path probed (/, /openapi.json, /swagger.json, /docs, /health).\n    No origin is currently serving this hostname.\ndomains:\n- domain: kafene.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kafene/refs/heads/main/security/kafene-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial-Services
- Fintech
- Lease-to-Own
- Point-of-Sale
- Consumer Finance
- Retail
- Underwriting
- Payments
---
