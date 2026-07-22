---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: route.com
  spf: true
hosts:
- cert_expires: Oct  9 07:17:26 2026 GMT
  host: route.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Route Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Route, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Route
provider_slug: route
slug: route-domain-security
source_filename: route-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: route.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 07:17:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: route.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/route/refs/heads/main/security/route-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SaaS
- E-commerce
- Shipping
- Package Tracking
- Shipping Protection
- Returns
- Post-Purchase
- Logistics
---
