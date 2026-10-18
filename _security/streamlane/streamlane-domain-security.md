---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getstreamlane.com
  spf: true
hosts:
- cert_expires: Jan  7 15:04:45 2027 GMT
  host: www.getstreamlane.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Streamlane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Streamlane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Streamlane
provider_slug: streamlane
slug: streamlane-domain-security
source_filename: streamlane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getstreamlane.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 15:04:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getstreamlane.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamlane/refs/heads/main/security/streamlane-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Parcel
- Logistics
- Software-as-a-Service
- Retail
- 3PL
---
