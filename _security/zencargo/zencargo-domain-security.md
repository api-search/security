---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_subdomain_policy: none
  dnssec: false
  domain: zencargo.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:mailgun.org ~all
hosts:
- cert_expires: Sep  2 06:31:18 2026 GMT
  cert_issuer: Google Trust Services (WR3)
  host: zencargo.com
  hsts: false
  https: true
  notes: Apex returns 301 redirect to www; no HSTS header observed on apex.
  tls_version: TLSv1.3
- cert_expires: Oct  2 01:26:23 2026 GMT
  cert_issuer: Google Trust Services (WR3)
  host: api-docs.zencargo.com
  hsts: false
  https: true
  notes: Static GraphQL API documentation served from Google Cloud Storage.
  tls_version: TLSv1.3
- cert_expires: Sep 23 18:02:47 2026 GMT
  cert_issuer: Google Trust Services (WR3)
  host: graphql.zencargo.com
  hsts: false
  https: true
  notes: Live Apollo Router GraphQL gateway; unauthenticated requests get CSRF-preflight / auth-gated errors.
  tls_version: TLSv1.3
- cert_expires: Sep 23 18:02:47 2026 GMT
  cert_issuer: Google Trust Services (WR3)
  host: app.zencargo.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  notes: Web application (API key & webhook management).
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zencargo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zencargo, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zencargo
provider_slug: zencargo
slug: zencargo-domain-security
source_filename: zencargo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + documentation/API hosts\nhosts:\n- host: zencargo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WR3)\n  cert_expires: Sep  2 06:31:18 2026 GMT\n  hsts: false\n  notes: Apex returns 301 redirect to www; no HSTS header observed on apex.\n- host: api-docs.zencargo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WR3)\n  cert_expires: Oct  2 01:26:23 2026 GMT\n  hsts: false\n  notes: Static GraphQL API documentation served from Google Cloud Storage.\n- host: graphql.zencargo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WR3)\n  cert_expires: Sep 23 18:02:47 2026 GMT\n  hsts: false\n  notes: Live Apollo Router GraphQL gateway; unauthenticated requests get CSRF-preflight / auth-gated errors.\n- host: app.zencargo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services\
  \ (WR3)\n  cert_expires: Sep 23 18:02:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  notes: Web application (API key & webhook management).\ndomains:\n- domain: zencargo.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:mailgun.org ~all\n  dmarc: true\n  dmarc_policy: none\n  dmarc_subdomain_policy: none\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zencargo/refs/heads/main/security/zencargo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Freight Forwarding
- Supply Chain
- Logistics
- Ocean Freight
- Shipment Tracking
- Bookings
- Supply Chain Visibility
- Freight
- SaaS
- GraphQL
---
