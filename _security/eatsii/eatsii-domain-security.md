---
description: ''
domains:
- caa: []
  created: '2024-12-31'
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: eatsii.com
  ds_records: []
  expires: '2026-12-31'
  mx: []
  nameservers:
  - ns1.domain.com
  - ns2.domain.com
  registrar: Network Solutions, LLC
  spf: false
hosts:
- host: eatsii.com
  hsts: false
  hsts_max_age: null
  http: true
  http_server: parking (208.91.197.27, Network Solutions)
  http_status: 200
  https: false
  tls_error: tlsv1 alert internal error (no peer certificate)
  tls_version: null
kind: domain-security
layout: security
method: probed
name: Eatsii Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eatsii, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Eatsii
provider_slug: eatsii
slug: eatsii-domain-security
source_filename: eatsii-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS + TLS + HTTP probe of eatsii.com (2026-07-20)\nnotes: >-\n  eatsii.com does not terminate TLS — port 443 aborts the handshake with a\n  TLSv1 internal error and presents no certificate. Port 80 answers from a\n  Network Solutions parking address (208.91.197.27) with a 195-byte\n  \"Error. Page cannot be displayed.\" page. DNS is wildcarded: every probed\n  subdomain (www, api, docs, developer, developers, status, trust, app)\n  resolves to the same parking IP, and every probed path returns HTTP 200\n  with that identical error body (verified soft-404 against a control path).\n  No mail, sender-authentication, or certificate-authority policy records\n  are published.\nhosts:\n- host: eatsii.com\n  https: false\n  tls_version: null\n  tls_error: tlsv1 alert internal error (no peer certificate)\n  http: true\n  http_status: 200\n  http_server: parking (208.91.197.27, Network Solutions)\n  hsts: false\n  hsts_max_age: null\n\
  domains:\n- domain: eatsii.com\n  dnssec: false\n  ds_records: []\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n  mx: []\n  nameservers:\n  - ns1.domain.com\n  - ns2.domain.com\n  registrar: Network Solutions, LLC\n  created: '2024-12-31'\n  expires: '2026-12-31'\nwildcard_dns: true\nwell_known_probed:\n- path: /.well-known/security.txt\n  status: 200\n  real: false\n  note: soft-404 parking page\n- path: /.well-known/openid-configuration\n  status: 200\n  real: false\n  note: soft-404 parking page\n- path: /.well-known/oauth-authorization-server\n  status: 200\n  real: false\n  note: soft-404 parking page\n- path: /.well-known/api-catalog\n  status: 200\n  real: false\n  note: soft-404 parking page\n- path: /.well-known/ai-plugin.json\n  status: 200\n  real: false\n  note: soft-404 parking page\n- path: /llms.txt\n  status: 200\n  real: false\n  note: soft-404 parking page\n- path: /openapi.json\n  status: 200\n  real: false\n  note: soft-404 parking page\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eatsii/refs/heads/main/security/eatsii-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Food and Beverage
- Cloud Kitchen
- Food Delivery
- Restaurants
- Foodtech
- Indonesia
- Southeast Asia
---
