---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aurora.tech
  spf: true
hosts:
- cert_expires: Aug 24 20:34:08 2026 GMT
  host: aurora.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aurora Innovation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aurora Innovation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aurora Innovation
provider_slug: aurora-innovation
slug: aurora-innovation-domain-security
source_filename: aurora-innovation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aurora.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 20:34:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aurora.tech\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aurora-innovation/refs/heads/main/security/aurora-innovation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Autonomous Vehicles
- Autonomous Trucking
- Self-Driving
- Freight
- Lidar
- FMCW
- NASDAQ
- Aurora Driver
---
