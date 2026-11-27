---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mcpal.io
  spf: true
hosts:
- cert_expires: Dec 23 10:43:14 2026 GMT
  host: mcpal.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MCPal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MCPal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MCPal
provider_slug: mcpal-io
slug: mcpal-io-domain-security
source_filename: mcpal-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcpal.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 10:43:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mcpal.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mcpal-io/security/mcpal-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Authentication
- OAuth
- Metering
- Subscription
- Payments
---
