---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tryhungry.com
  spf: true
hosts:
- cert_expires: Oct 14 05:27:54 2026 GMT
  host: tryhungry.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 05:44:29 2026 GMT
  host: api.tryhungry.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: Private first-party API host behind Cloudflare. Answers a Go-style plain-text "404 page not found" on every probed path; no public documentation or specification is served here.
  tls_version: TLSv1.3
- cert_expires: Oct 28 08:07:52 2026 GMT
  host: admin.tryhungry.com
  hsts: false
  https: true
  note: Internal admin single-page app; answers 200 with an HTML shell for every path including /.well-known/*.
  tls_version: TLSv1.3
- cert_expires: Oct 20 13:03:42 2026 GMT
  host: gamma.tryhungry.com
  hsts: false
  https: true
  note: Marketing/pop-ups single-page app; answers 200 with an HTML shell for every path including /.well-known/*.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hungry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HUNGRY, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HUNGRY
provider_slug: hungry
slug: hungry-domain-security
source_filename: hungry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts plus the first-party api./admin./gamma. subdomains\n  discovered during contract discovery\nhosts:\n- host: tryhungry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 05:27:54 2026 GMT\n  hsts: false\n- host: api.tryhungry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 05:44:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: Private first-party API host behind Cloudflare. Answers a Go-style plain-text \"404 page not found\"\n    on every probed path; no public documentation or specification is served here.\n- host: admin.tryhungry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 08:07:52 2026 GMT\n  hsts: false\n  note: Internal admin single-page app; answers 200 with an HTML shell for every path including /.well-known/*.\n- host: gamma.tryhungry.com\n  https: true\n\
  \  tls_version: TLSv1.3\n  cert_expires: Oct 20 13:03:42 2026 GMT\n  hsts: false\n  note: Marketing/pop-ups single-page app; answers 200 with an HTML shell for every path including /.well-known/*.\ndomains:\n- domain: tryhungry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\nfindings:\n- Only api.tryhungry.com sets Strict-Transport-Security; the apex tryhungry.com, admin. and gamma. do\n  not.\n- tryhungry.com publishes no CAA record and DNSSEC is not enabled on the zone.\n- SPF and DMARC are both published, but the DMARC policy is p=none (monitor only, no enforcement).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hungry/refs/heads/main/security/hungry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Food and Beverage
- Catering
- Marketplace
- Logistics
- Food Delivery
- Workplace
- Hospitality
- Corporate Services
- Last Mile Delivery
---
