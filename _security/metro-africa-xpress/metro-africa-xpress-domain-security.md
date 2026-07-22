---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: maxdrive.ai
  spf: true
hosts:
- cert_expires: Aug 28 12:57:33 2026 GMT
  host: www.maxdrive.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metro Africa Xpress Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metro Africa Xpress, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Metro Africa Xpress
provider_slug: metro-africa-xpress
slug: metro-africa-xpress-domain-security
source_filename: metro-africa-xpress-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.maxdrive.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 12:57:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: maxdrive.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metro-africa-xpress/refs/heads/main/security/metro-africa-xpress-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mobility
- Transportation
- Electric Vehicles
- Vehicle Financing
- Logistics
- Fintech
- Africa
- Nigeria
---
