---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mrsuppy.com
  spf: true
hosts:
- cert_expires: Jan 31 08:43:27 2027 GMT
  host: mrsuppy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mr Suppy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mr Suppy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Mr Suppy
provider_slug: mrsuppy-com
slug: mrsuppy-com-domain-security
source_filename: mrsuppy-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mrsuppy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 08:43:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mrsuppy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mrsuppy-com/security/mrsuppy-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Supplements
- Price Comparison
- E-Commerce
- Health
- United Kingdom
---
