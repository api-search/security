---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apmzoom.com
  spf: true
hosts:
- cert_expires: Jan  3 14:06:18 2027 GMT
  host: apmzoom.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apmzoom Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for apM Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: apM Group
provider_slug: apmzoom-com
slug: apmzoom-com-domain-security
source_filename: apmzoom-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apmzoom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 14:06:18 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: apmzoom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/apmzoom-com/security/apmzoom-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fashion
- Wholesale
- South Korea
- Marketplace
- Artificial Intelligence
---
