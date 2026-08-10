---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rokid.com
  spf: true
hosts:
- cert_expires: Feb  3 08:30:20 2027 GMT
  host: www.rokid.com
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 08:30:20 2027 GMT
  host: x-docs.rokid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 08:30:20 2027 GMT
  host: api.rokid.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 10:27:32 2026 GMT
  host: global.rokid.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 08:30:20 2027 GMT
  host: open.rokid.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 08:30:20 2027 GMT
  host: maven.rokid.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  3 08:30:20 2027 GMT
  host: openapi.rokid.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15724800
  https: true
  note: every path answers HTTP 401 anonymously
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rokid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rokid, probed live across 7 host(s) and 1 registrable domain(s). 7 host(s) serve HTTPS (up to TLSv1.3); 6 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rokid
provider_slug: rokid
slug: rokid-domain-security
source_filename: rokid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rokid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 08:30:20 2027 GMT\n  hsts: true\n  hsts_max_age: 5184000\n- host: x-docs.rokid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 08:30:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rokid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 08:30:20 2027 GMT\n  hsts: null\n- host: global.rokid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 10:27:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n  hsts_include_subdomains: false\n- host: open.rokid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 08:30:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: maven.rokid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 08:30:20 2027 GMT\n  hsts:\
  \ true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: openapi.rokid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  3 08:30:20 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\n  hsts_include_subdomains: true\n  note: every path answers HTTP 401 anonymously\nfindings:\n- api.rokid.com — the production API host — sends no Strict-Transport-Security\n  header, while every other Rokid host does.\n- maven.rokid.com and openapi.rokid.com negotiate TLS 1.2 rather than 1.3.\n- rokid.com publishes no CAA records and DNSSEC is not enabled.\n- The DMARC record is published with p=none, so it monitors without enforcing.\ndomains:\n- domain: rokid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rokid/refs/heads/main/security/rokid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Smart Glasses
- Augmented Reality
- Wearables
- Artificial Intelligence
- Spatial Computing
- Device Management
- Consumer Electronics
- Voice
- Enterprise
- Hardware
- Agents
---
