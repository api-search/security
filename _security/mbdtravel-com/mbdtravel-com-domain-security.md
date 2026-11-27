---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mbdtravel.com
  spf: true
hosts:
- cert_expires: Dec 26 13:58:39 2026 GMT
  host: mbdtravel.com
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MBD Travel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MBD Travel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MBD Travel
provider_slug: mbdtravel-com
slug: mbdtravel-com-domain-security
source_filename: mbdtravel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mbdtravel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 13:58:39 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: mbdtravel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mbdtravel-com/security/mbdtravel-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Tourism
- United Arab Emirates
- Tours
- Visa
---
