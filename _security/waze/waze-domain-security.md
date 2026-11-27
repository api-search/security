---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: waze.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Jan 22 14:15:11 2027 GMT
  host: waze.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 20:39:28 2027 GMT
  host: embed.waze.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Waze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Waze, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Waze
provider_slug: waze
slug: waze-domain-security
source_filename: waze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: waze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 14:15:11 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: embed.waze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 20:39:28 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: waze.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/waze/security/waze-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobility
- Navigation
- Maps
- Traffic
- Location
- Transportation
- Smart Cities
---
