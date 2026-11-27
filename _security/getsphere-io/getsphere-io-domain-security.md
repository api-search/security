---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getsphere.io
  spf: false
hosts:
- cert_expires: Dec 26 00:03:54 2026 GMT
  host: getsphere.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sphere Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sphere, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Sphere
provider_slug: getsphere-io
slug: getsphere-io-domain-security
source_filename: getsphere-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getsphere.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 00:03:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: getsphere.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getsphere-io/security/getsphere-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FoodTracking
- Health
- Nutrition
- Mobile App
- Lifestyle
---
