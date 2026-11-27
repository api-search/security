---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: parcellaunch.com
  spf: true
hosts:
- cert_expires: Jan 15 02:03:05 2027 GMT
  host: parcellaunch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ParcelLaunch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ParcelLaunch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ParcelLaunch
provider_slug: parcellaunch-com
slug: parcellaunch-com-domain-security
source_filename: parcellaunch-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parcellaunch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 02:03:05 2027 GMT\n  hsts: false\ndomains:\n- domain: parcellaunch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/parcellaunch-com/security/parcellaunch-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- 3D Visualization
- Property Marketing
- Software-as-a-Service
---
