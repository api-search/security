---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: parcelmonitor.com
  spf: true
hosts:
- cert_expires: Sep 10 08:34:41 2026 GMT
  host: www.parcelmonitor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.parcelmonitor.com
  https: false
kind: domain-security
layout: security
method: probed
name: Parcel Monitor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parcel Monitor, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Parcel Monitor
provider_slug: parcel-monitor
slug: parcel-monitor-domain-security
source_filename: parcel-monitor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.parcelmonitor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 08:34:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.parcelmonitor.com\n  https: false\ndomains:\n- domain: parcelmonitor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parcel-monitor/refs/heads/main/security/parcel-monitor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Shipping
- Package Tracking
- Logistics
- Carriers
- Delivery
- Webhooks
- E-Commerce
---
