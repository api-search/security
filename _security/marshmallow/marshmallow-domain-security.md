---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: marshmallow.com
  spf: true
hosts:
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: www.marshmallow.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: auth.marshmallow.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: authorization server
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: api.marshmallow.com
  hsts: false
  https: true
  role: private application API
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: account.marshmallow.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  role: consumer account portal
  tls_version: TLSv1.3
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: docs.marshmallow.com
  hsts: false
  https: true
  role: gated docs distribution (403 anonymous)
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Marshmallow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marshmallow, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Marshmallow
provider_slug: marshmallow
slug: marshmallow-domain-security
source_filename: marshmallow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.marshmallow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: false\n- host: auth.marshmallow.com\n  role: authorization server\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: api.marshmallow.com\n  role: private application API\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: false\n- host: account.marshmallow.com\n  role: consumer account portal\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n- host: docs.marshmallow.com\n  role: gated docs distribution (403 anonymous)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n\
  \  hsts: false\ndomains:\n- domain: marshmallow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nnotes:\n- >-\n  Extended on 2026-07-25 beyond the script's apis.yml-derived host list to cover\n  the four other live Marshmallow hosts (auth., api., account., docs.), each\n  probed directly over TLS and HTTP HEAD.\n- >-\n  HSTS is enforced on the two hosts that handle user credentials\n  (auth., account.) but not on www., api. or docs.\n- No CAA records and no DNSSEC on marshmallow.com; SPF present and DMARC at p=reject.\n- No RFC 9116 security.txt is published on any host (see well-known/marshmallow-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marshmallow/refs/heads/main/security/marshmallow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- United Kingdom
- Insurtech
- Property and Casualty
- Motor Insurance
- Home Insurance
- Telematics
- Underwriting
- Claims
- Direct to Consumer
- Partner Gated
- No Public API
---
