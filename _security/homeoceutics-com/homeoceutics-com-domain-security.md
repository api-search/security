---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: homeoceutics.com
  spf: true
hosts:
- cert_expires: Jan 24 02:56:23 2027 GMT
  host: homeoceutics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Homeoceutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Homeoceutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Homeoceutics
provider_slug: homeoceutics-com
slug: homeoceutics-com-domain-security
source_filename: homeoceutics-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: homeoceutics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 02:56:23 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: homeoceutics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/homeoceutics-com/security/homeoceutics-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Health
- Wellness
- DigitalCatalogue
- French
---
