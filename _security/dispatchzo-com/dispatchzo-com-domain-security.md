---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dispatchzo.com
  spf: true
hosts:
- cert_expires: Feb  1 01:34:38 2027 GMT
  host: dispatchzo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dispatchzo Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dispatchzo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dispatchzo
provider_slug: dispatchzo-com
slug: dispatchzo-com-domain-security
source_filename: dispatchzo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dispatchzo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 01:34:38 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dispatchzo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dispatchzo-com/security/dispatchzo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Field Service Scheduling
- Dispatch Software
- Small Business Software
- Pricing Tools
---
