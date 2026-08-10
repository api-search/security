---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: serenaandlily.com
  spf: true
hosts:
- cert_expires: Sep 21 03:51:37 2026 GMT
  host: www.serenaandlily.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 63072000
  hsts_preload: false
  https: true
  note: HTTP 403 (DataDome bot challenge) is returned to non-browser clients for HTML routes, so the automated probe recorded hsts as null. The header was verified directly on both the 403 root response and a 404 route response — strict-transport-security is present with max-age=63072000.
  server: Vercel
  tls_version: TLSv1.3
  x_frame_options: DENY
- host: api.serenaandlily.com
  https: true
  note: Amazon API Gateway. Every path probed returns HTTP 403 {"message":"Missing Authentication Token"}; no anonymous surface.
  reachable: true
kind: domain-security
layout: security
method: probed
name: Serena Lily Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Serena & Lily, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Serena & Lily
provider_slug: serena-lily
slug: serena-lily-domain-security
source_filename: serena-lily-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (probe-domain-security.py, plus manual\n  header verification because the marketing host answers a DataDome bot challenge)\nhosts:\n- host: www.serenaandlily.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:51:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: false\n  hsts_preload: false\n  x_frame_options: DENY\n  server: Vercel\n  note: >-\n    HTTP 403 (DataDome bot challenge) is returned to non-browser clients for HTML routes,\n    so the automated probe recorded hsts as null. The header was verified directly on both\n    the 403 root response and a 404 route response — strict-transport-security is present\n    with max-age=63072000.\n- host: api.serenaandlily.com\n  https: true\n  reachable: true\n  note: >-\n    Amazon API Gateway. Every path probed returns HTTP 403 {\"message\":\"Missing\n    Authentication Token\"}; no anonymous\
  \ surface.\ndomains:\n- domain: serenaandlily.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nfindings:\n- id: hsts-present\n  status: pass\n  detail: strict-transport-security max-age=63072000 (2 years) on www.serenaandlily.com.\n- id: dmarc-enforcing\n  status: pass\n  detail: _dmarc.serenaandlily.com publishes \"v=DMARC1; p=reject;\" — full enforcement.\n- id: tls-modern\n  status: pass\n  detail: TLSv1.3 negotiated.\n- id: dnssec-absent\n  status: fail\n  detail: No DS record published for serenaandlily.com; the zone is not DNSSEC signed.\n- id: caa-absent\n  status: fail\n  detail: No CAA record published; any CA may issue for serenaandlily.com.\n- id: hsts-no-subdomains\n  status: warn\n  detail: >-\n    HSTS does not assert includeSubDomains, so api.serenaandlily.com and other subdomains\n    are not covered by the policy, and the domain is not preload-eligible.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/serena-lily/refs/heads/main/security/serena-lily-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- E-Commerce
- Home Furnishings
- Furniture
- Interior Design
- Home Decor
- Direct to Consumer
---
