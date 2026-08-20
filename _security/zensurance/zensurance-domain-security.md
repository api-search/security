---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zensurance.com
  spf: true
hosts:
- cert_expires: Oct 13 05:47:10 2026 GMT
  host: www.zensurance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  headers:
    x_content_type_options: nosniff
    x_frame_options: SAMEORIGIN
  host: api.zensurance.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  https: true
  note: Undocumented first-party backend. Probed manually because it is not carried in apis.yml apis[] (it is not a published product API). Negotiates TLS 1.2 only — an explicit TLS 1.3 handshake is refused.
  tls13_supported: false
  tls_version: TLSv1.2
- cert_expires: Oct 26 23:59:59 2026 GMT
  headers:
    x_content_type_options: nosniff
  host: app.zensurance.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: Customer application (S3-fronted SPA). TLS 1.2 only.
  server: AmazonS3
  tls13_supported: false
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zensurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zensurance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zensurance
provider_slug: zensurance
slug: zensurance-domain-security
source_filename: zensurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zensurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 05:47:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.zensurance.com\n  https: true\n  tls_version: TLSv1.2\n  tls13_supported: false\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  headers:\n    x_content_type_options: nosniff\n    x_frame_options: SAMEORIGIN\n  note: Undocumented first-party backend. Probed manually because it is not carried\n    in apis.yml apis[] (it is not a published product API). Negotiates TLS 1.2 only —\n    an explicit TLS 1.3 handshake is refused.\n- host: app.zensurance.com\n  https: true\n  tls_version: TLSv1.2\n  tls13_supported: false\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload:\
  \ true\n  server: AmazonS3\n  headers:\n    x_content_type_options: nosniff\n  note: Customer application (S3-fronted SPA). TLS 1.2 only.\ndomains:\n- domain: zensurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zensurance/refs/heads/main/security/zensurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Canada
- Insurtech
- Brokers
- Property and Casualty
- Commercial Insurance
- Small Business Insurance
- Cyber Insurance
- Digital Brokerage
- Partner Gated
---
