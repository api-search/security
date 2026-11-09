---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: asgolfclothing.com
  spf: false
hosts:
- cert_expires: Dec  5 00:30:52 2026 GMT
  host: asgolfclothing.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asgolfclothing Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Black Label Golf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Black Label Golf
provider_slug: asgolfclothing-com
slug: asgolfclothing-com-domain-security
source_filename: asgolfclothing-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asgolfclothing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 00:30:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: asgolfclothing.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/asgolfclothing-com/security/asgolfclothing-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Golf
- Apparel
- Fashion
- E-Commerce
- Sports
---
