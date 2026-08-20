---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: smart-data.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; rua=mailto:REDACTED@dmarc-reports.cloudflare.net
  dnssec: false
  domain: ndsmartdata.com
  note: Probed by hand 2026-08-14. This is the domain SmartData actually operates the product and its mail on; smart-data.com is the marketing front and carries no SPF, DMARC, CAA or DNSSEC at all. DMARC on ndsmartdata.com is at p=none, i.e. monitoring only - no enforcement against spoofed mail.
  spf: true
  spf_record: v=spf1 include:spf.protection.outlook.com -all
hosts:
- cert_expires: Oct 20 08:52:37 2026 GMT
  host: www.smart-data.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: app.ndsmartdata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: The SmartData application host (nginx 1.30.3, Django/DRF). Added by hand on 2026-08-14 because apis.yml carries no apis[] entry for it - SmartData ships no public API - so the automated probe, which walks apis.yml baseURLs and OpenAPI servers[], never reaches it. Response also sets X-Frame-Options DENY, X-Content-Type-Options nosniff, Referrer-Policy same-origin and Cross-Origin-Opener-Policy same-origin.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smart Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SmartData, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: SmartData
provider_slug: smart-data
slug: smart-data-domain-security
source_filename: smart-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smart-data.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 08:52:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.ndsmartdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: >-\n    The SmartData application host (nginx 1.30.3, Django/DRF). Added by hand on\n    2026-08-14 because apis.yml carries no apis[] entry for it - SmartData ships no\n    public API - so the automated probe, which walks apis.yml baseURLs and OpenAPI\n    servers[], never reaches it. Response also sets X-Frame-Options DENY,\n    X-Content-Type-Options nosniff, Referrer-Policy same-origin and\n    Cross-Origin-Opener-Policy same-origin.\ndomains:\n- domain: smart-data.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: ndsmartdata.com\n  dnssec:\
  \ false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.protection.outlook.com -all\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record: v=DMARC1; p=none; rua=mailto:REDACTED@dmarc-reports.cloudflare.net\n  note: >-\n    Probed by hand 2026-08-14. This is the domain SmartData actually operates the\n    product and its mail on; smart-data.com is the marketing front and carries no SPF,\n    DMARC, CAA or DNSSEC at all. DMARC on ndsmartdata.com is at p=none, i.e. monitoring\n    only - no enforcement against spoofed mail.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smart-data/refs/heads/main/security/smart-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Drone Data
- Geospatial
- Asset Inspection
- Photogrammetry
- LiDAR
- Point Cloud
- 3D Visualization
- Gaussian Splatting
- Computer-Vision
- Infrastructure
- Utilities
- Mining
- Forestry
- Australia
---
