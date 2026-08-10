---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: freetrade.io
  spf: true
hosts:
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: freetrade.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  server: cloudflare
  tls_version: TLSv1.3
- csp: true
  host: web.freetrade.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: Authenticated web trading platform; strict CSP with nonce + strict-dynamic.
  server: cloudflare
  tls_version: TLSv1.3
  x_content_type_options: nosniff
- csp: true
  host: help.freetrade.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: Intercom-hosted help centre (CNAME); response headers are Intercom's, not Freetrade's.
  server: cloudflare
  tls_version: TLSv1.3
  x_content_type_options: nosniff
  x_frame_options: DENY
kind: domain-security
layout: security
method: probed
name: Freetrade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freetrade, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Freetrade
provider_slug: freetrade
slug: freetrade-domain-security
source_filename: freetrade-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freetrade.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  server: cloudflare\n- host: web.freetrade.io\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  csp: true\n  x_content_type_options: nosniff\n  server: cloudflare\n  note: Authenticated web trading platform; strict CSP with nonce + strict-dynamic.\n- host: help.freetrade.io\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  csp: true\n  x_frame_options: DENY\n  x_content_type_options: nosniff\n  server: cloudflare\n  note: Intercom-hosted help centre (CNAME); response headers are Intercom's, not Freetrade's.\n\
  domains:\n- domain: freetrade.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\ngaps:\n- No DNSSEC on freetrade.io.\n- No CAA records on freetrade.io.\nx-evidence:\n  fetched: '2026-08-04'\n  method: dig + openssl s_client + curl -I\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freetrade/refs/heads/main/security/freetrade-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Investing
- Stock Trading
- Brokerage
- Financial Services
- Fintech
- Pensions
- ISA
- Personal Finance
- United Kingdom
---
