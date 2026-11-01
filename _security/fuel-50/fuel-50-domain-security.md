---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fuel50.com
  spf: true
hosts:
- cert_expires: Jan 22 03:10:22 2027 GMT
  host: fuel50.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fuel 50 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fuel 50, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fuel 50
provider_slug: fuel-50
slug: fuel-50-domain-security
source_filename: fuel-50-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fuel50.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 03:10:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fuel50.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fuel-50/security/fuel-50-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Workforce
- Scheduling
- TimeTracking
- LaborCompliance
---
