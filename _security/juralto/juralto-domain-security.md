---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: juralto.com
  spf: false
hosts:
- cert_expires: Dec 23 12:03:46 2026 GMT
  host: juralto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Juralto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juralto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Juralto
provider_slug: juralto
slug: juralto-domain-security
source_filename: juralto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: juralto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 12:03:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: juralto.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/juralto/security/juralto-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fintech
- Payments
- API
- Infrastructure
---
