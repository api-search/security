---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: snapshyft.com
  spf: false
hosts:
- cert_expires: Sep 17 19:51:54 2026 GMT
  host: snapshyft.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snapshyft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SnapShyft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: SnapShyft
provider_slug: snapshyft
slug: snapshyft-domain-security
source_filename: snapshyft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snapshyft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:51:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: snapshyft.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapshyft/refs/heads/main/security/snapshyft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Staffing
- Workforce
- Marketplace
- Gig Economy
- Hospitality
- On-Demand
---
